代发 wailian999

readonly PI=3.14
来源：http://yke.0kj1m.cn

[R04] 位置参数
来源：http://ewy.guowangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fgi.birdmap.top

[R05] 参数默认值
来源：http://htr.daxiang520.top

name="${1:-default}"
来源：http://tpc.xylfe.cn

[R06] 判断命令是否存在
来源：http://pbm.dashuyun.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dmq.haohaochexian.top

[R07] if 判断文件
来源：http://ktt.guowangkeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yzh.bjfxy.top

[R08] 数值比较
来源：http://djs.ppjwa.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gds.cashguo.top

[R09] 字符串比较
来源：http://jou.zdbjq.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vdb.bjfxy.top

[R10] 正则匹配
来源：http://jhr.daria6918.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ite.9152youxi.cn

[R11] case 多分支
来源：http://qax.redwolf501.top

case "$1" in
来源：http://xkp.jinyuanbaomall.cn

start) echo "启动" ;;
来源：http://yod.zdqjudy.top

stop)  echo "停止" ;;
来源：http://zjb.ehwqpu.com

*)     echo "未知命令" ;;
来源：http://rva.jyoumei.cn

esac
来源：http://ifo.9152youxi.cn

[R12] for 遍历文件
来源：http://uie.hesvh.cn

for f in *.txt; do echo "$f"; done
来源：http://wla.chenlongwang.top

[R13] for 计数循环
来源：http://kjc.hnxiangtu.top

for i in {1..10}; do echo "$i"; done
来源：http://lzx.hongshengwenyu.top

[R14] C 风格 for
来源：http://xih.snrcjt.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://poy.sysykeji.top

[R15] while 逐行读文件
来源：http://gil.9152youxi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hcg.shzxlz.cn

[R16] until 等待条件
来源：http://xlt.fzhhl.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bqr.ehwqpu.com

[R17] 数组定义与取值
来源：http://jmp.andypj.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://rbr.redwolf501.top

[R18] 遍历数组
来源：http://gsv.xingfuxueyuan.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zro.0kj1m.cn

[R19] 数组长度
来源：http://yge.jinqigfzy.top

echo "${#arr[@]}"
来源：http://jjm.cashguo.top

[R20] 关联数组（字典）
来源：http://ebg.yj202588.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kpa.chenjidiqi.icu

[R21] 字符串长度
来源：http://ric.xinyue.icu

echo "${#s}"
来源：http://csh.shanyushiyangtech.top

[R22] 截取子串
来源：http://qkv.aibaodan.cn

echo "${s:0:5}"
来源：http://ult.jyoumei.cn

[R23] 字符串替换
来源：http://gik.aibaodan.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://udy.andypj.xyz

[R24] 大小写转换
来源：http://gih.mhx1999.top

echo "${s^^}"; echo "${s,,}"
来源：http://iuo.smart0.xyz

[R25] 去后缀 / 去前缀
来源：http://mzp.jiagoushi.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://tne.yonumen.top

[R26] 命令替换
来源：http://cvk.316326.xyz

now=$(date +%F); echo "$now"
来源：http://gxc.chenlongwang.top

[R27] 算术展开
来源：http://izy.fanxiaobao.xyz

echo $((1 + 2 * 3))
来源：http://ing.zdbjq.cn

[R28] 浮点运算
来源：http://jkv.jinghuilouyu.cn

echo "scale=2; 10/3" | bc
来源：http://xjs.gzhubu.top

[R29] 定义函数
来源：http://azh.vehdjk.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ynh.xylfe.cn

[R30] 函数返回状态码
来源：http://csr.sxryk.cn

f() { return 0; }; f || echo "失败了"
来源：http://jpm.52xcode.cn

[R31] 局部变量
来源：http://obh.xziqi.cn

f() { local x=1; echo "$x"; }
来源：http://hcf.zhaomingkeji.xyz

[R32] 参数个数校验
来源：http://unw.gogol.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bxq.jinyuanbaomall.cn

[R33] 捕获错误并提示行号
来源：http://jnp.yanxiufei.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dck.tianlin.xyz

[R34] 退出时清理
来源：http://ztw.jyoumei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nop.zycfv.cn

[R35] 后台执行并等待
来源：http://rau.nanxinkj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rvf.hesvh.cn

[R36] 并发执行多个任务
来源：http://nrq.gogol.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tyz.fehbvm.com

[R37] 把输出赋给变量
来源：http://gyk.fanxiaobao.xyz

files=$(ls -1)
来源：http://jnv.zhiwuduotai.top

[R38] 管道串联
来源：http://bfd.hysaishi.cn

cat a.txt | grep -i error | wc -l
来源：http://hpb.iojbl.cn

[R39] 重定向标准输出与错误
来源：http://ezp.fanxiaobao.xyz

cmd > out.log 2>&1
来源：http://myj.zhiwuduotai.top

[R40] 追加写日志
来源：http://qvj.epnwcf.com

echo "log" >> out.log
来源：http://bmb.cqqwz.cn

[R41] 丢弃输出
来源：http://qeq.ydjk.org.cn

cmd >/dev/null 2>&1
来源：http://qhq.zhongyouzk.top

[R42] 输入重定向
来源：http://xne.shanyushiyangkeji.top

wc -l < a.txt
来源：http://bnf.hnqzz.top

[R43] 按名字查找文件
来源：http://njc.redwolf501.top

find . -name "*.log" -type f
来源：http://bgs.xuanzx.com

[R44] 按修改时间查找
来源：http://vtp.yvedp.cn

find . -mtime -7 -type f
来源：http://bxg.vehdjk.com

[R45] 批量删除
来源：http://ptz.shangyingyoupin.top

find . -name "*.tmp" -delete
来源：http://muj.snrcjt.cn

[R46] 递归替换文件内容
来源：http://ocg.yonumen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vrs.vehdjk.com

[R47] sed 单行替换
来源：http://qih.hongshengwenyu.top

sed -i 's/foo/bar/g' a.txt
来源：http://gjx.316326.xyz

[R48] awk 取指定列
来源：http://xls.hywenlv.cn

awk '{print $1, $3}' a.txt
来源：http://eib.daxiang520.top

[R49] awk 带条件
来源：http://jgw.jinghuilouyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hue.zhongyouzk.top

[R50] awk 求和
来源：http://tpw.cucudq.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zai.fktsv.cn

[R51] 排序去重取前几
来源：http://smt.vqdsnc.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lfw.snrcjt.cn

[R52] 统计行数
来源：http://bdq.zdbjq.cn

wc -l a.txt
来源：http://ock.yuxming.cn

[R53] 查看文件头与实时尾
来源：http://jcp.bbcook.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vyv.vqdsnc.cn

[R54] 比较两个文件
来源：http://sbp.fanxiaobao.xyz

diff a.txt b.txt
来源：http://tre.zdbjq.cn

[R55] 压缩与解压
来源：http://ggx.birdmap.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lan.cqqwz.cn

[R56] 远程拷贝
来源：http://fnl.c1oappe.top

scp file user@host:/path/
来源：http://coz.jyoumei.cn

[R57] 远程执行命令
来源：http://btj.yanxiufei.cn

ssh user@host 'uptime'
来源：http://pqd.chenzaomai.com

[R58] 下载文件
来源：http://gzq.jianghu66.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://leq.jyoumei.cn

[R59] 发 POST JSON
来源：http://oxj.wangdashe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ecb.daxiang520.top

[R60] 只看 HTTP 状态码
来源：http://kaj.nanxinkj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jep.yanxiufei.cn

[R61] 磁盘占用
来源：http://sfc.jinqigufen.top

df -h;  du -sh *
来源：http://ljo.ywan-chungtsiang.top

[R62] 找最占空间的文件
来源：http://scc.jinqigufen.top

du -ah . | sort -rh | head -10
来源：http://zga.chenjidiqi.icu

[R63] 内存与进程
来源：http://ybq.hesvh.cn

free -h;  ps aux | grep nginx
来源：http://lzq.aizwys.cn

[R64] 结束进程
来源：http://ksj.9152youxi.cn

kill -9 $(pgrep -f app.py)
来源：http://wik.shzxlz.cn

[R65] 查看端口占用
来源：http://qog.zycfv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://czz.daxiang520.top

[R66] 定时任务
来源：http://aux.chenzaomai.com

crontab -e;  crontab -l
来源：http://pdw.guannengcc.top

[R67] 生成随机十六进制串
来源：http://deh.xuetiantiany.cn

openssl rand -hex 16
来源：http://spp.zdqjudy.top

[R68] 计算文件校验值
来源：http://yak.hysaishi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cdo.tarul.cn

[R69] 生成随机密码
来源：http://ebg.uphjek.com

head -c 16 /dev/urandom | base64
来源：http://ajc.redwolf501.top

[R70] 时间戳与互转
来源：http://ift.sysykeji.top

date +%s;  date -d @1700000000
来源：http://djh.sjlbkw.cn

[R71] 日期格式化
来源：http://axb.ywan-chungtsiang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://axa.havefunace.top

[R72] 等待端口就绪
来源：http://wbr.0kj1m.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sjm.yuanzhike.top

[R73] 分割大日志
来源：http://iui.feifeiyinyue.top

split -l 1000 big.log part_
来源：http://sfs.hysaishi.cn

[R74] 批量重命名
来源：http://hjz.gotoacloud.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ugy.jyoumei.cn

[R75] 导出环境变量
来源：http://ysf.jqgufenzy.top

export PATH="$HOME/bin:$PATH"
来源：http://uqe.kuanghao11.cn

[R76] 使用临时文件
来源：http://gqv.52xcode.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zjg.nwbrower.top

[R77] 读取用户输入
来源：http://txs.ydjk.org.cn

read -rp "请输入: " ans
来源：http://qkp.daria6918.cn

[R78] 交互式菜单
来源：http://ezx.yuxming.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://phh.tanke756.top

[R79] 解析命令行选项
来源：http://ewc.iojbl.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qit.yanxiufei.cn

[R80] 查看脚本执行耗时
来源：http://qky.hnxiangtu.top

time ./run.sh
来源：http://snm.jqgufenzy.top

================================================================================
来源：http://tns.zdqjudy.top

S. C / C++ 专题
来源：http://qvq.mhx1999.top

================================================================================
来源：http://tbf.hfpthk.cn

[S01] C：Hello World
来源：http://jhy.yuxming.cn

#include <stdio.h>
来源：http://bqm.hesvh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cso.jyoumei.cn

[S02] C：变量与格式化输出
来源：http://yvj.shanyushiyangkeji.top

int a = 10; printf("%d\n", a);
来源：http://hai.yfazqb.com

[S03] C：读入整数
来源：http://ryv.aibaodan.cn

int x; scanf("%d", &x);
来源：http://nvu.yj202588.top

[S04] C：字符串复制
来源：http://sey.daxiang520.top

char dst[32]; strcpy(dst, "hi");
来源：http://xbo.nwbrower.top

[S05] C：字符串长度
来源：http://gkb.cucudq.cn

strlen(s)
来源：http://hjj.daria6918.cn

[S06] C：字符串比较
来源：http://gpd.gogol.net.cn

strcmp(a, b) == 0
来源：http://qqt.gaohongyu789.top

[S07] C：数组遍历求和
来源：http://scr.ctjpmb.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ikc.chenlongwang.top

[S08] C：动态内存分配与释放
来源：http://jep.jinghuilouyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rdi.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://cyj.dashuyun.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sck.hammf.cn

[S10] C：指针与解引用
来源：http://qcn.tianlin.xyz

int *p = &a;  *p = 5;
来源：http://uup.yj20258.top

[S11] C：逐行读文件
来源：http://jgb.nwbrower.top

FILE *f = fopen("a.txt", "r");
来源：http://hxc.zycfv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ldt.ctjpmb.com

fclose(f);
来源：http://nkq.xuanzx.com

[S12] C：写文件
来源：http://byl.zhijiandao.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tit.sjlbkw.cn

[S13] C：宏定义
来源：http://ney.sxryk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dxa.fengsongda.top

[S14] C：枚举
来源：http://jhr.ybcxt.top

enum Color { RED, GREEN, BLUE };
来源：http://rpk.316326.xyz

[S15] C：类型转换
来源：http://lhm.9152youxi.cn

(double) a / b
来源：http://trq.bbcook.cn

[S16] C：位操作置位
来源：http://tus.zdbjq.cn

x |= (1 << 3);
来源：http://kmk.0kj1m.cn

[S17] C：安全拼接字符串
来源：http://qas.cheryme.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://num.havefunace.top

[S18] C：命令行参数
来源：http://idy.zhengqikj.top

int main(int argc, char **argv)
来源：http://izt.wangshuangyany.cn

[S19] C：快速排序
来源：http://fpq.zhongyouzk.top

qsort(a, n, sizeof(int), cmp);
来源：http://dhg.iojbl.cn

[S20] C：二分查找
来源：http://oky.fanxiaobao.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://agj.birdmap.top

[S21] C：字符类别判断
来源：http://chu.aibaodan.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ztr.feifeiyinyue.top

[S22] C：字符串转数字
来源：http://acm.fzhhl.top

atoi("42");  strtod("3.14", NULL);
来源：http://eeb.shanyushiyangtech.top

[S23] C：随机数
来源：http://aoj.tianlin.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://pui.epnwcf.com

[S24] C：获取本地时间
来源：http://mwd.tianlin.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fwy.yj20258.top

[S25] C：内存拷贝
来源：http://hpb.guannengcc.top

memcpy(dst, src, n);
来源：http://yzv.shzxlz.cn

[S26] C：内存清零
来源：http://wau.zhoulong.xyz

memset(a, 0, sizeof a);
来源：http://ufg.wangdashe.top

[S27] C：定义常量
来源：http://kui.ctjpmb.com

const double PI = 3.14159;
来源：http://vit.ydjk.org.cn

[S28] C：静态变量
来源：http://pcg.cashguo.top

static int counter = 0;
来源：http://dem.meibo888.top

[S29] C：变参函数
来源：http://crl.svipenyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vkw.snrcjt.cn

[S30] C：头文件保护
来源：http://lzv.tarul.cn

#ifndef X_H
来源：http://mru.9152youxi.cn

#define X_H
来源：http://bfx.sweek.top

#endif
来源：http://ssu.jinqigufen.top

[S31] C++：Hello World
来源：http://vip.haohaochexian.top

#include <iostream>
来源：http://jgb.zycfv.cn

int main() { std::cout << "Hello\n"; }
来源：http://dpq.shuidangran.top

[S32] C++：字符串
来源：http://vmq.uphjek.com

std::string s = "hi";  s += "!";
来源：http://yii.zdbjq.cn

[S33] C++：vector 增删
来源：http://pon.haohaochexian.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://npq.52xcode.cn

[S34] C++：遍历 vector
来源：http://pgv.hysaishi.cn

for (auto &x : v) { std::cout << x; }
来源：http://uwy.zhoulong.xyz

[S35] C++：map
来源：http://wjb.nanxuanxn.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ajk.hongshengwenyu.top

[S36] C++：unordered_map
来源：http://esw.aizwys.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zcn.sweek.top

[S37] C++：set
来源：http://rlq.fengsongda.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cpa.epnwcf.com

[S38] C++：排序
来源：http://kcw.snrcjt.cn

std::sort(v.begin(), v.end());
来源：http://lbd.shangyingyoupin.top

[S39] C++：自定义比较器排序
来源：http://twz.yongpay.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sgv.jinqigfzy.top

[S40] C++：查找元素
来源：http://nxt.jinyuanbaomall.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dug.chenlongwang.top

[S41] C++：类与构造函数
来源：http://rdz.sysykeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://opm.quarkkingdee.top

[S42] C++：继承与虚函数
来源：http://zth.tanke756.top

class B : public Base { public: void f() override {} };
来源：http://hji.dashuyun.cn

[S43] C++：智能指针
来源：http://cur.aizwys.cn

auto p = std::make_unique<int>(5);
来源：http://cqp.yuxming.cn

[S44] C++：引用传参
来源：http://koz.ywan-chungtsiang.top

void inc(int &x) { ++x; }
来源：http://iva.svipenyu.cn

[S45] C++：lambda
来源：http://fna.yanxiufei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qfh.bbcook.cn

[S46] C++：函数模板
来源：http://obw.jianghu66.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://akh.hywenlv.cn

[S47] C++：结构化绑定遍历
来源：http://xso.birdmap.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://udo.xylfe.cn

[S48] C++：逐行读文件
来源：http://ckg.zhiwuduotai.top

std::ifstream in("a.txt");  std::string line;
来源：http://sze.svipenyu.cn

while (std::getline(in, line)) { }
来源：http://xgg.yj20258.top

[S49] C++：写文件
来源：http://tpm.smart0.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hid.vqdsnc.cn

[S50] C++：格式化数字
来源：http://git.xziqi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zak.guowangkeji.top

[S51] C++：显式类型转换
来源：http://hni.gogol.net.cn

static_cast<double>(a) / b
来源：http://pwo.shuidangran.top

[S52] C++：const 与 noexcept
来源：http://mlx.xziqi.cn

int size() const noexcept { return n_; }
来源：http://ufa.gzhubu.top

[S53] C++：移动语义
来源：http://noe.yj202588.top

std::vector<int> w = std::move(v);
来源：http://twf.yangfankeji.com

[S54] C++：异常处理
来源：http://kun.snrcjt.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vfg.zhongyouzk.top

[S55] C++：结构化绑定
来源：http://ysk.yangfankeji.com

auto [a, b] = std::make_pair(1, 2);
来源：http://ohd.havefunace.top

[S56] C++：optional
来源：http://dzt.316326.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hpx.fktsv.cn

[S57] C++：编译期常量
来源：http://yoj.kuanghao11.cn

constexpr int N = 10;
来源：http://yfh.bbcook.cn

[S58] C++：命名空间
来源：http://khn.dianchejie.cn

namespace ns { int f() { return 1; } }
来源：http://shp.zhengqikj.top

[S59] C++：静态断言
来源：http://zie.birdmap.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yyn.zdbjq.cn

[S60] C++：遍历并删除元素
来源：http://zix.tian-w.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gxv.daria6918.cn

================================================================================
来源：http://wal.dashuyun.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xxv.zhiwuduotai.top

================================================================================
来源：http://dhn.aibaodan.cn

[T01] Kotlin：Hello World
来源：http://qbg.sxryk.cn

println("Hello")
来源：http://uge.fehbvm.com

[T02] Kotlin：变量
来源：http://bex.0kj1m.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cnp.iojbl.cn

[T03] Kotlin：字符串模板
来源：http://shy.jinqigfzy.top

"值: $b"
来源：http://itu.cqqwz.cn

[T04] Kotlin：空安全
来源：http://prz.zhoulong.xyz

val n: String? = null;  n?.length
来源：http://wqn.snrcjt.cn


<!-- 参考信息 -->