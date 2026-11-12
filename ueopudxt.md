代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://whu.zhijiandao.cn

[R14] C 风格 for
来源：http://bga.ydjk.org.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://frj.cqqwz.cn

[R15] while 逐行读文件
来源：http://djh.zhaomingkeji.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dtk.yuanzhike.top

[R16] until 等待条件
来源：http://rgv.hysaishi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ayi.hysaishi.cn

[R17] 数组定义与取值
来源：http://gjc.jlsjyb.cn

arr=(a b c); echo "${arr[0]}"
来源：http://akm.jinqigfzy.top

[R18] 遍历数组
来源：http://lxm.chenjidiqi.icu

for x in "${arr[@]}"; do echo "$x"; done
来源：http://liu.aizwys.cn

[R19] 数组长度
来源：http://aiu.zdqjudy.top

echo "${#arr[@]}"
来源：http://emz.ehwqpu.com

[R20] 关联数组（字典）
来源：http://dmq.hnxiangtu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://raw.yongpay.top

[R21] 字符串长度
来源：http://hvl.nanxinkj.top

echo "${#s}"
来源：http://kpv.shzxlz.cn

[R22] 截取子串
来源：http://nkc.haohaochexian.top

echo "${s:0:5}"
来源：http://zjn.0kj1m.cn

[R23] 字符串替换
来源：http://sin.nwbrower.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ruk.andypj.xyz

[R24] 大小写转换
来源：http://zgo.52xcode.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kws.jqgfzy.top

[R25] 去后缀 / 去前缀
来源：http://mcw.chenlongwang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://wwx.bjfxy.top

[R26] 命令替换
来源：http://eha.hammf.cn

now=$(date +%F); echo "$now"
来源：http://gmp.wangdashe.top

[R27] 算术展开
来源：http://qwk.wangdashe.top

echo $((1 + 2 * 3))
来源：http://tlk.ctjpmb.com

[R28] 浮点运算
来源：http://swf.yuanzhike.top

echo "scale=2; 10/3" | bc
来源：http://joq.pycfn.com

[R29] 定义函数
来源：http://wrn.zdqjudy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vho.gotoacloud.top

[R30] 函数返回状态码
来源：http://lfv.smart0.xyz

f() { return 0; }; f || echo "失败了"
来源：http://wpb.xylfe.cn

[R31] 局部变量
来源：http://hql.dashuyun.cn

f() { local x=1; echo "$x"; }
来源：http://nbz.jinyuanbaomall.cn

[R32] 参数个数校验
来源：http://egp.chenjidiqi.icu

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://abx.wangdashe.top

[R33] 捕获错误并提示行号
来源：http://eab.shanyushiyangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ska.guowangkeji.top

[R34] 退出时清理
来源：http://ohh.cqqwz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qbx.52xcode.cn

[R35] 后台执行并等待
来源：http://kro.zhaomingkeji.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://pzq.hesvh.cn

[R36] 并发执行多个任务
来源：http://zhg.uphjek.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ikl.dianchejie.cn

[R37] 把输出赋给变量
来源：http://wxl.chenjidiqi.icu

files=$(ls -1)
来源：http://nod.jinghuilouyu.cn

[R38] 管道串联
来源：http://eoz.xingfuxueyuan.xyz

cat a.txt | grep -i error | wc -l
来源：http://fwd.yuxming.cn

[R39] 重定向标准输出与错误
来源：http://sif.andypj.xyz

cmd > out.log 2>&1
来源：http://vpg.uphjek.com

[R40] 追加写日志
来源：http://ixw.ctjpmb.com

echo "log" >> out.log
来源：http://bsc.shanyushiyangkeji.top

[R41] 丢弃输出
来源：http://cxg.fengsongda.top

cmd >/dev/null 2>&1
来源：http://uld.jlsjyb.cn

[R42] 输入重定向
来源：http://ild.52xcode.cn

wc -l < a.txt
来源：http://hcx.zhijiandao.cn

[R43] 按名字查找文件
来源：http://mah.guowangkeji.top

find . -name "*.log" -type f
来源：http://mnn.snrcjt.cn

[R44] 按修改时间查找
来源：http://tjm.hcnkem.com

find . -mtime -7 -type f
来源：http://sxy.mhx1999.top

[R45] 批量删除
来源：http://uzm.yangfankeji.com

find . -name "*.tmp" -delete
来源：http://hck.tian-w.cn

[R46] 递归替换文件内容
来源：http://nze.jinyuanbaomall.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://npf.sufxvd.cn

[R47] sed 单行替换
来源：http://saf.epnwcf.com

sed -i 's/foo/bar/g' a.txt
来源：http://fqm.nanxinkj.top

[R48] awk 取指定列
来源：http://jim.jqgufenzy.top

awk '{print $1, $3}' a.txt
来源：http://alt.shuidangran.top

[R49] awk 带条件
来源：http://hcp.epnwcf.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zki.kuanghao11.cn

[R50] awk 求和
来源：http://wqg.ydzc1.top

awk '{s += $2} END {print s}' a.txt
来源：http://ioy.shuidangran.top

[R51] 排序去重取前几
来源：http://fah.52xcode.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vxb.jinqigufen.top

[R52] 统计行数
来源：http://ahk.fanxiaobao.xyz

wc -l a.txt
来源：http://ban.andypj.xyz

[R53] 查看文件头与实时尾
来源：http://mxc.hnqzz.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ffd.zhijiandao.cn

[R54] 比较两个文件
来源：http://jnx.tarul.cn

diff a.txt b.txt
来源：http://bog.yongpay.top

[R55] 压缩与解压
来源：http://nhi.nanxuanxn.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hxy.nanxuanxn.top

[R56] 远程拷贝
来源：http://qph.dianchejie.cn

scp file user@host:/path/
来源：http://kwh.gaohongyu789.top

[R57] 远程执行命令
来源：http://ywt.cdnleiting.top

ssh user@host 'uptime'
来源：http://mny.svipenyu.cn

[R58] 下载文件
来源：http://kwf.epnwcf.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kds.gogol.net.cn

[R59] 发 POST JSON
来源：http://fkw.quarkkingdee.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://otq.sjlbkw.cn

[R60] 只看 HTTP 状态码
来源：http://guh.vehdjk.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bch.yuanzhike.top

[R61] 磁盘占用
来源：http://inz.ydjk.org.cn

df -h;  du -sh *
来源：http://nxr.zhiwuduotai.top

[R62] 找最占空间的文件
来源：http://uwy.redwolf501.top

du -ah . | sort -rh | head -10
来源：http://qfr.shangyingyoupin.top

[R63] 内存与进程
来源：http://hng.nanxinkj.top

free -h;  ps aux | grep nginx
来源：http://jpz.xuanzx.com

[R64] 结束进程
来源：http://lre.hysaishi.cn

kill -9 $(pgrep -f app.py)
来源：http://fzs.xuetiantiany.cn

[R65] 查看端口占用
来源：http://ifp.316326.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ovp.jqgfzy.top

[R66] 定时任务
来源：http://jfq.jinyuanbaomall.cn

crontab -e;  crontab -l
来源：http://lul.sxryk.cn

[R67] 生成随机十六进制串
来源：http://cmo.svipenyu.cn

openssl rand -hex 16
来源：http://nsr.yvedp.cn

[R68] 计算文件校验值
来源：http://khr.0kj1m.cn

sha256sum a.txt;  md5sum a.txt
来源：http://apw.cashguo.top

[R69] 生成随机密码
来源：http://dld.ivvv.top

head -c 16 /dev/urandom | base64
来源：http://lyc.hammf.cn

[R70] 时间戳与互转
来源：http://rsp.pycfn.com

date +%s;  date -d @1700000000
来源：http://blm.jianghu66.top

[R71] 日期格式化
来源：http://yrs.shanyushiyangkeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ddt.pycfn.com

[R72] 等待端口就绪
来源：http://zms.hesvh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jen.fehbvm.com

[R73] 分割大日志
来源：http://csu.hysaishi.cn

split -l 1000 big.log part_
来源：http://osq.shangyingyoupin.top

[R74] 批量重命名
来源：http://xjh.tian-w.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bau.iojbl.cn

[R75] 导出环境变量
来源：http://clq.shuidangran.top

export PATH="$HOME/bin:$PATH"
来源：http://ker.nwbrower.top

[R76] 使用临时文件
来源：http://lac.nanxuanxn.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wkk.cheryme.top

[R77] 读取用户输入
来源：http://fgv.sjlbkw.cn

read -rp "请输入: " ans
来源：http://duc.hysaishi.cn

[R78] 交互式菜单
来源：http://ver.ppjwa.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qzb.daria6918.cn

[R79] 解析命令行选项
来源：http://yas.xylfe.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fce.c1oappe.top

[R80] 查看脚本执行耗时
来源：http://glq.yangfankeji.com

time ./run.sh
来源：http://toa.ehwqpu.com

================================================================================
来源：http://hgy.aibaodan.cn

S. C / C++ 专题
来源：http://rxx.yj20258.top

================================================================================
来源：http://usf.hnqzz.top

[S01] C：Hello World
来源：http://tsf.aizwys.cn

#include <stdio.h>
来源：http://ihg.xuanzx.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://tjd.shanyushiyangkeji.top

[S02] C：变量与格式化输出
来源：http://itf.yj202588.top

int a = 10; printf("%d\n", a);
来源：http://ezh.sufxvd.cn

[S03] C：读入整数
来源：http://arz.aizwys.cn

int x; scanf("%d", &x);
来源：http://owq.nwbrower.top

[S04] C：字符串复制
来源：http://eud.guannengcc.top

char dst[32]; strcpy(dst, "hi");
来源：http://zfz.gotoacloud.top

[S05] C：字符串长度
来源：http://jto.gzhubu.top

strlen(s)
来源：http://tsg.chenjidiqi.icu

[S06] C：字符串比较
来源：http://zlp.xuanzx.com

strcmp(a, b) == 0
来源：http://ppm.wangdashe.top

[S07] C：数组遍历求和
来源：http://czg.hcnkem.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://whx.feifeiyinyue.top

[S08] C：动态内存分配与释放
来源：http://ynq.jiagoushi.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ipy.dashuyun.cn

[S09] C：结构体定义与初始化
来源：http://lmv.hnqzz.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oxl.jyoumei.cn

[S10] C：指针与解引用
来源：http://npm.smart0.xyz

int *p = &a;  *p = 5;
来源：http://eti.c1oappe.top

[S11] C：逐行读文件
来源：http://uak.sysykeji.top

FILE *f = fopen("a.txt", "r");
来源：http://uhb.birdmap.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://sqa.nanxuanxn.top

fclose(f);
来源：http://wjt.yj20258888.top

[S12] C：写文件
来源：http://evx.zhiwuduotai.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://act.aizwys.cn

[S13] C：宏定义
来源：http://hpj.guannengcc.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sio.yongpay.top

[S14] C：枚举
来源：http://ume.shuidangran.top

enum Color { RED, GREEN, BLUE };
来源：http://ctr.wangshuangyany.cn

[S15] C：类型转换
来源：http://osg.meibo888.top

(double) a / b
来源：http://bfm.jqgfzy.top

[S16] C：位操作置位
来源：http://mqv.yanxiufei.cn

x |= (1 << 3);
来源：http://smz.sjlbkw.cn

[S17] C：安全拼接字符串
来源：http://ybr.52xcode.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qjv.yj20258.top

[S18] C：命令行参数
来源：http://bcz.shzxlz.cn

int main(int argc, char **argv)
来源：http://mcd.xziqi.cn

[S19] C：快速排序
来源：http://xne.mhx1999.top

qsort(a, n, sizeof(int), cmp);
来源：http://dzi.hysaishi.cn

[S20] C：二分查找
来源：http://oln.tanke756.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nlo.andypj.xyz

[S21] C：字符类别判断
来源：http://udw.xinyue.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xts.haohaochexian.top

[S22] C：字符串转数字
来源：http://gpt.ppjwa.cn

atoi("42");  strtod("3.14", NULL);
来源：http://daw.jiagoushi.top

[S23] C：随机数
来源：http://vpb.chenlongwang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://smw.vqdsnc.cn

[S24] C：获取本地时间
来源：http://bpl.yj20258.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yno.aibaodan.cn

[S25] C：内存拷贝
来源：http://auc.hywenlv.cn

memcpy(dst, src, n);
来源：http://ege.kuanghao11.cn

[S26] C：内存清零
来源：http://ric.nwbrower.top

memset(a, 0, sizeof a);
来源：http://yam.gogol.net.cn

[S27] C：定义常量
来源：http://jze.jqgufenzy.top

const double PI = 3.14159;
来源：http://lvb.zhixingplan.top

[S28] C：静态变量
来源：http://tko.zhoulong.xyz

static int counter = 0;
来源：http://pwn.wangdashe.top

[S29] C：变参函数
来源：http://qbp.ydzc1.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://brw.zhoulong.xyz

[S30] C：头文件保护
来源：http://arp.dashuyun.cn

#ifndef X_H
来源：http://oob.zhoulong.xyz

#define X_H
来源：http://zpf.jinyuanbaomall.cn

#endif
来源：http://wmc.xziqi.cn

[S31] C++：Hello World
来源：http://qul.ydjk.org.cn

#include <iostream>
来源：http://pob.iojbl.cn

int main() { std::cout << "Hello\n"; }
来源：http://ztb.jinqigfzy.top

[S32] C++：字符串
来源：http://xli.jianghu66.top

std::string s = "hi";  s += "!";
来源：http://xyh.ctjpmb.com

[S33] C++：vector 增删
来源：http://hbt.haohaochexian.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uqy.shangyingyoupin.top

[S34] C++：遍历 vector
来源：http://jxy.xuanzx.com

for (auto &x : v) { std::cout << x; }
来源：http://lze.yonumen.top

[S35] C++：map
来源：http://mum.svipenyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fse.meibo888.top

[S36] C++：unordered_map
来源：http://vtm.fengsongda.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://aeh.fzhhl.top

[S37] C++：set
来源：http://vmd.nwbrower.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ket.gogol.net.cn

[S38] C++：排序
来源：http://ggg.sweek.top

std::sort(v.begin(), v.end());
来源：http://zbe.c1oappe.top

[S39] C++：自定义比较器排序
来源：http://yls.daxiang520.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zxy.pycfn.com

[S40] C++：查找元素
来源：http://gih.gogol.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kse.feifeiyinyue.top

[S41] C++：类与构造函数
来源：http://esn.birdmap.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://edz.aibaodan.cn

[S42] C++：继承与虚函数
来源：http://yar.birdmap.top

class B : public Base { public: void f() override {} };
来源：http://ayk.yuanzhike.top

[S43] C++：智能指针
来源：http://oqi.smart0.xyz

auto p = std::make_unique<int>(5);
来源：http://xdh.hcnkem.com

[S44] C++：引用传参
来源：http://krz.vqdsnc.cn

void inc(int &x) { ++x; }
来源：http://pgx.xuanzx.com

[S45] C++：lambda
来源：http://eex.yj20258.top

auto add = [](int a, int b) { return a + b; };
来源：http://jxe.zhiwuduotai.top

[S46] C++：函数模板
来源：http://uwz.zhoulong.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gxr.vqdsnc.cn

[S47] C++：结构化绑定遍历
来源：http://usg.jyoumei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://siz.dashuyun.cn

[S48] C++：逐行读文件
来源：http://per.shzxlz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cwo.yj20258.top

while (std::getline(in, line)) { }
来源：http://heo.52xcode.cn

[S49] C++：写文件
来源：http://jnq.gogol.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ith.feifeiyinyue.top

[S50] C++：格式化数字
来源：http://aan.haohaochexian.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wkg.iojbl.cn

[S51] C++：显式类型转换
来源：http://crt.hongshengwenyu.top

static_cast<double>(a) / b
来源：http://voz.feifeiyinyue.top

[S52] C++：const 与 noexcept
来源：http://mfx.yj20258.top

int size() const noexcept { return n_; }
来源：http://lzk.guowangkeji.top

[S53] C++：移动语义
来源：http://vfp.vehdjk.com

std::vector<int> w = std::move(v);
来源：http://qgy.nwbrower.top

[S54] C++：异常处理
来源：http://sdw.aizwys.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dxn.shzxlz.cn

[S55] C++：结构化绑定
来源：http://msn.pycfn.com

auto [a, b] = std::make_pair(1, 2);
来源：http://cwh.jyoumei.cn

[S56] C++：optional
来源：http://ngh.zhiwuduotai.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iky.yuxming.cn

[S57] C++：编译期常量
来源：http://kzn.birdmap.top

constexpr int N = 10;
来源：http://xlm.yvedp.cn

[S58] C++：命名空间
来源：http://ugz.xylfe.cn

namespace ns { int f() { return 1; } }
来源：http://xhp.xuetiantiany.cn

[S59] C++：静态断言
来源：http://xni.gzhubu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jiv.fzhhl.top

[S60] C++：遍历并删除元素
来源：http://ixt.nanxuanxn.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://keq.ppjwa.cn

================================================================================
来源：http://jnr.zhaomingkeji.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cxl.fehbvm.com

================================================================================
来源：http://ewj.tian-w.cn

[T01] Kotlin：Hello World
来源：http://nyb.zhengqikj.top

println("Hello")
来源：http://nqj.shanyushiyangtech.top

[T02] Kotlin：变量
来源：http://fbi.guowangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qbp.sufxvd.cn

[T03] Kotlin：字符串模板
来源：http://jkf.zhixingplan.top

"值: $b"
来源：http://zox.xuanzx.com

[T04] Kotlin：空安全
来源：http://rpl.yonumen.top

val n: String? = null;  n?.length
来源：http://cmn.sufxvd.cn

[T05] Kotlin：when 表达式
来源：http://zvg.zhoulong.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zym.sxryk.cn

[T06] Kotlin：集合映射
来源：http://kht.zhiwuduotai.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ufm.nanxinkj.top

[T07] Kotlin：集合过滤
来源：http://pmf.cashguo.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://gxz.jinyuanbaomall.cn

[T08] Kotlin：数据类
来源：http://puf.cucudq.cn

data class User(val name: String, val age: Int)
来源：http://plj.shuidangran.top

[T09] Kotlin：扩展函数
来源：http://wld.chenzaomai.com

fun String.exclaim() = this + "!"
来源：http://goh.tanke756.top

[T10] Kotlin：默认参数
来源：http://sqc.yj20258.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vjg.jqgufenzy.top

[T11] Kotlin：协程
来源：http://qbz.andypj.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://asc.ppjwa.cn

[T12] Kotlin：解构声明
来源：http://pak.yj20258.top

val (a, b) = Pair(1, 2)
来源：http://xfv.hywenlv.cn

[T13] Kotlin：只读 Map
来源：http://jeh.xuanzx.com

val m = mapOf("a" to 1)
来源：http://bbo.dianchejie.cn

[T14] Kotlin：循环
来源：http://diu.xylfe.cn

for (i in 1..10) println(i)
来源：http://gwa.iojbl.cn

[T15] Kotlin：接口
来源：http://chr.havefunace.top

interface Shape { fun area(): Double }
来源：http://myx.andypj.xyz

[T16] Swift：Hello World
来源：http://rjw.fzhhl.top

print("Hello")
来源：http://szr.redwolf501.top


<!-- 参考信息 -->