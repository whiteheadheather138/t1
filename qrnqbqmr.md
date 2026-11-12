代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yxn.zhixingplan.top

[R08] 数值比较
来源：http://gav.sufxvd.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ede.xuetiantiany.cn

[R09] 字符串比较
来源：http://maj.ehwqpu.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ovf.ivvv.top

[R10] 正则匹配
来源：http://iqj.nanxuanxn.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rxm.yonumen.top

[R11] case 多分支
来源：http://tcm.gogol.net.cn

case "$1" in
来源：http://ngr.cheryme.top

start) echo "启动" ;;
来源：http://apx.jlsjyb.cn

stop)  echo "停止" ;;
来源：http://nod.yj202588.top

*)     echo "未知命令" ;;
来源：http://bsi.uphjek.com

esac
来源：http://avo.redwolf501.top

[R12] for 遍历文件
来源：http://whc.hywenlv.cn

for f in *.txt; do echo "$f"; done
来源：http://ywk.fanxiaobao.xyz

[R13] for 计数循环
来源：http://rws.gogol.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://vmm.mhx1999.top

[R14] C 风格 for
来源：http://drt.sweek.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xra.ywan-chungtsiang.top

[R15] while 逐行读文件
来源：http://lyr.hnxiangtu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gzo.fanxiaobao.xyz

[R16] until 等待条件
来源：http://qik.yueranfly.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://djd.chenjidiqi.icu

[R17] 数组定义与取值
来源：http://pcp.uphjek.com

arr=(a b c); echo "${arr[0]}"
来源：http://mjt.52xcode.cn

[R18] 遍历数组
来源：http://jxy.tianlin.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uua.zhoulong.xyz

[R19] 数组长度
来源：http://isq.havefunace.top

echo "${#arr[@]}"
来源：http://nfd.jlsjyb.cn

[R20] 关联数组（字典）
来源：http://qnc.snrcjt.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ewv.0kj1m.cn

[R21] 字符串长度
来源：http://dhf.ppjwa.cn

echo "${#s}"
来源：http://xbt.tanke756.top

[R22] 截取子串
来源：http://blw.vqdsnc.cn

echo "${s:0:5}"
来源：http://uiu.9152youxi.cn

[R23] 字符串替换
来源：http://vvh.havefunace.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://drz.snrcjt.cn

[R24] 大小写转换
来源：http://wov.zhaomingkeji.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://pfh.jinghuilouyu.cn

[R25] 去后缀 / 去前缀
来源：http://ooj.svipenyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://amf.andypj.xyz

[R26] 命令替换
来源：http://fna.zhixingplan.top

now=$(date +%F); echo "$now"
来源：http://plx.chenzaomai.com

[R27] 算术展开
来源：http://yjh.fzhhl.top

echo $((1 + 2 * 3))
来源：http://qxj.zycfv.cn

[R28] 浮点运算
来源：http://fkm.yueranfly.top

echo "scale=2; 10/3" | bc
来源：http://ivg.pycfn.com

[R29] 定义函数
来源：http://ngr.andypj.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ntz.fktsv.cn

[R30] 函数返回状态码
来源：http://bpw.jinghuilouyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://qvs.sxryk.cn

[R31] 局部变量
来源：http://uvd.xingfuxueyuan.xyz

f() { local x=1; echo "$x"; }
来源：http://zhp.zdbjq.cn

[R32] 参数个数校验
来源：http://xib.jinyuanbaomall.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cug.cqqwz.cn

[R33] 捕获错误并提示行号
来源：http://vyy.jinghuilouyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hmv.gogol.net.cn

[R34] 退出时清理
来源：http://mqh.shanyushiyangkeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://zjg.svipenyu.cn

[R35] 后台执行并等待
来源：http://pun.bbcook.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lva.chenlongwang.top

[R36] 并发执行多个任务
来源：http://hty.ehwqpu.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bqt.bjfxy.top

[R37] 把输出赋给变量
来源：http://ffv.pengpengdd.cyou

files=$(ls -1)
来源：http://jrp.xylfe.cn

[R38] 管道串联
来源：http://inf.vqdsnc.cn

cat a.txt | grep -i error | wc -l
来源：http://obn.ybcxt.top

[R39] 重定向标准输出与错误
来源：http://ufz.dianchejie.cn

cmd > out.log 2>&1
来源：http://zqh.andypj.xyz

[R40] 追加写日志
来源：http://uqz.fengsongda.top

echo "log" >> out.log
来源：http://udi.yj202588.top

[R41] 丢弃输出
来源：http://aod.zhongyouzk.top

cmd >/dev/null 2>&1
来源：http://gvv.xylfe.cn

[R42] 输入重定向
来源：http://bkv.haohaochexian.top

wc -l < a.txt
来源：http://puu.shuidangran.top

[R43] 按名字查找文件
来源：http://lsm.fehbvm.com

find . -name "*.log" -type f
来源：http://rnk.shanyushiyangkeji.top

[R44] 按修改时间查找
来源：http://zdl.zhongyouzk.top

find . -mtime -7 -type f
来源：http://kan.shanyushiyangkeji.top

[R45] 批量删除
来源：http://hux.guowangkeji.top

find . -name "*.tmp" -delete
来源：http://gsb.bjfxy.top

[R46] 递归替换文件内容
来源：http://qop.tanke756.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vrr.yangfankeji.com

[R47] sed 单行替换
来源：http://dgm.sysykeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://jai.fktsv.cn

[R48] awk 取指定列
来源：http://exa.hesvh.cn

awk '{print $1, $3}' a.txt
来源：http://fmo.sufxvd.cn

[R49] awk 带条件
来源：http://ujc.yanxiufei.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://viq.nwbrower.top

[R50] awk 求和
来源：http://aee.zycfv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mti.jiagoushi.top

[R51] 排序去重取前几
来源：http://krt.chenlongwang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://aky.yonumen.top

[R52] 统计行数
来源：http://mem.redwolf501.top

wc -l a.txt
来源：http://ovx.andypj.xyz

[R53] 查看文件头与实时尾
来源：http://eag.wangshuangyany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pma.zhiwuduotai.top

[R54] 比较两个文件
来源：http://qfb.c1oappe.top

diff a.txt b.txt
来源：http://fpf.jinyuanbaomall.cn

[R55] 压缩与解压
来源：http://ili.yj20258.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://amv.pycfn.com

[R56] 远程拷贝
来源：http://flg.tian-w.cn

scp file user@host:/path/
来源：http://ufe.vehdjk.com

[R57] 远程执行命令
来源：http://qaf.chenlongwang.top

ssh user@host 'uptime'
来源：http://etz.bjfxy.top

[R58] 下载文件
来源：http://spi.yangfankeji.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qiy.feifeiyinyue.top

[R59] 发 POST JSON
来源：http://pnx.yvedp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dnm.gotoacloud.top

[R60] 只看 HTTP 状态码
来源：http://gyh.jinqigufen.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oiv.fzhhl.top

[R61] 磁盘占用
来源：http://wnt.fzhhl.top

df -h;  du -sh *
来源：http://epd.zhiwuduotai.top

[R62] 找最占空间的文件
来源：http://gmq.jinqigufen.top

du -ah . | sort -rh | head -10
来源：http://plu.jqgfzy.top

[R63] 内存与进程
来源：http://swp.0kj1m.cn

free -h;  ps aux | grep nginx
来源：http://ane.xingfuxueyuan.xyz

[R64] 结束进程
来源：http://dij.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://syx.yuxming.cn

[R65] 查看端口占用
来源：http://xsr.yanxiufei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qjv.chenjidiqi.icu

[R66] 定时任务
来源：http://wfa.yvedp.cn

crontab -e;  crontab -l
来源：http://gyt.epnwcf.com

[R67] 生成随机十六进制串
来源：http://ytv.sxryk.cn

openssl rand -hex 16
来源：http://zwe.gaohongyu789.top

[R68] 计算文件校验值
来源：http://rei.tanke756.top

sha256sum a.txt;  md5sum a.txt
来源：http://zcr.jinqigufen.top

[R69] 生成随机密码
来源：http://hbr.yueranfly.top

head -c 16 /dev/urandom | base64
来源：http://irg.tian-w.cn

[R70] 时间戳与互转
来源：http://cpk.zdqjudy.top

date +%s;  date -d @1700000000
来源：http://itp.cheryme.top

[R71] 日期格式化
来源：http://nih.vqdsnc.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://anm.shzxlz.cn

[R72] 等待端口就绪
来源：http://djp.cucudq.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fui.shuidangran.top

[R73] 分割大日志
来源：http://ruj.hfpthk.cn

split -l 1000 big.log part_
来源：http://qpm.sxryk.cn

[R74] 批量重命名
来源：http://wmd.tian-w.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rlo.gzhubu.top

[R75] 导出环境变量
来源：http://vda.shangyingyoupin.top

export PATH="$HOME/bin:$PATH"
来源：http://tsg.bjfxy.top

[R76] 使用临时文件
来源：http://iww.hnqzz.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lwc.sweek.top

[R77] 读取用户输入
来源：http://uhs.nanxuanxn.top

read -rp "请输入: " ans
来源：http://rrv.daria6918.cn

[R78] 交互式菜单
来源：http://sqc.feifeiyinyue.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vei.fzhhl.top

[R79] 解析命令行选项
来源：http://tyx.snrcjt.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cld.hesvh.cn

[R80] 查看脚本执行耗时
来源：http://ibz.dianchejie.cn

time ./run.sh
来源：http://pzy.bbcook.cn

================================================================================
来源：http://eqg.ybcxt.top

S. C / C++ 专题
来源：http://xzo.wangdashe.top

================================================================================
来源：http://xjs.yfazqb.com

[S01] C：Hello World
来源：http://lda.gogol.net.cn

#include <stdio.h>
来源：http://yvk.ivvv.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mba.sufxvd.cn

[S02] C：变量与格式化输出
来源：http://doi.quarkkingdee.top

int a = 10; printf("%d\n", a);
来源：http://oek.yuanzhike.top

[S03] C：读入整数
来源：http://nna.yanxiufei.cn

int x; scanf("%d", &x);
来源：http://pld.hnqzz.top

[S04] C：字符串复制
来源：http://xjz.fktsv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dmv.feifeiyinyue.top

[S05] C：字符串长度
来源：http://qnm.wangshuangyany.cn

strlen(s)
来源：http://exz.jlsjyb.cn

[S06] C：字符串比较
来源：http://ewk.dashuyun.cn

strcmp(a, b) == 0
来源：http://kdp.9152youxi.cn

[S07] C：数组遍历求和
来源：http://rdx.shzxlz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vun.hfpthk.cn

[S08] C：动态内存分配与释放
来源：http://oth.hongshengwenyu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hoj.xingfuxueyuan.xyz

[S09] C：结构体定义与初始化
来源：http://ucc.zhaomingkeji.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ylm.guowangkeji.top

[S10] C：指针与解引用
来源：http://sei.shangyingyoupin.top

int *p = &a;  *p = 5;
来源：http://jcw.yonumen.top

[S11] C：逐行读文件
来源：http://zxe.tanke756.top

FILE *f = fopen("a.txt", "r");
来源：http://uns.hcnkem.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://ioe.jinqigfzy.top

fclose(f);
来源：http://jbz.sysykeji.top

[S12] C：写文件
来源：http://sps.yj20258.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iwp.bjfxy.top

[S13] C：宏定义
来源：http://eir.smart0.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jjm.xuanzx.com

[S14] C：枚举
来源：http://lln.jinqigfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://kkx.dianchejie.cn

[S15] C：类型转换
来源：http://rcl.jinghuilouyu.cn

(double) a / b
来源：http://qwq.epnwcf.com

[S16] C：位操作置位
来源：http://tib.kuanghao11.cn

x |= (1 << 3);
来源：http://odu.chenjidiqi.icu

[S17] C：安全拼接字符串
来源：http://cbs.meibo888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blx.nanxinkj.top

[S18] C：命令行参数
来源：http://wry.hysaishi.cn

int main(int argc, char **argv)
来源：http://nus.daria6918.cn

[S19] C：快速排序
来源：http://awi.meibo888.top

qsort(a, n, sizeof(int), cmp);
来源：http://ypx.hysaishi.cn

[S20] C：二分查找
来源：http://lgd.tarul.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ley.aizwys.cn

[S21] C：字符类别判断
来源：http://yua.ywan-chungtsiang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://luv.gzhubu.top

[S22] C：字符串转数字
来源：http://rdf.yj20258.top

atoi("42");  strtod("3.14", NULL);
来源：http://nsj.birdmap.top

[S23] C：随机数
来源：http://waj.52xcode.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bzj.daria6918.cn

[S24] C：获取本地时间
来源：http://ejg.yonumen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ami.zycfv.cn

[S25] C：内存拷贝
来源：http://jgg.xuanzx.com

memcpy(dst, src, n);
来源：http://rpi.guannengcc.top

[S26] C：内存清零
来源：http://byd.jqgfzy.top

memset(a, 0, sizeof a);
来源：http://utk.pycfn.com

[S27] C：定义常量
来源：http://qhy.gzhubu.top

const double PI = 3.14159;
来源：http://tbh.vqdsnc.cn

[S28] C：静态变量
来源：http://lyv.sufxvd.cn

static int counter = 0;
来源：http://rgn.zhaomingkeji.xyz

[S29] C：变参函数
来源：http://jbn.fktsv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://aib.yangfankeji.com

[S30] C：头文件保护
来源：http://fpi.shanyushiyangkeji.top

#ifndef X_H
来源：http://heu.yueranfly.top

#define X_H
来源：http://kkn.chenlongwang.top

#endif
来源：http://que.epnwcf.com

[S31] C++：Hello World
来源：http://rrx.zhongyouzk.top

#include <iostream>
来源：http://lbp.hnxiangtu.top

int main() { std::cout << "Hello\n"; }
来源：http://eha.shanyushiyangtech.top

[S32] C++：字符串
来源：http://mxl.xziqi.cn

std::string s = "hi";  s += "!";
来源：http://sug.0kj1m.cn

[S33] C++：vector 增删
来源：http://ckx.0kj1m.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qne.iojbl.cn

[S34] C++：遍历 vector
来源：http://zrv.0kj1m.cn

for (auto &x : v) { std::cout << x; }
来源：http://xjy.meibo888.top

[S35] C++：map
来源：http://xil.jiagoushi.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://juz.fehbvm.com

[S36] C++：unordered_map
来源：http://qkp.meibo888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wju.andypj.xyz

[S37] C++：set
来源：http://ffo.fehbvm.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jhv.ybcxt.top

[S38] C++：排序
来源：http://uhx.yvedp.cn

std::sort(v.begin(), v.end());
来源：http://jit.ctjpmb.com

[S39] C++：自定义比较器排序
来源：http://pnr.ehwqpu.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qyg.aizwys.cn

[S40] C++：查找元素
来源：http://tfp.cheryme.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lsh.zhijiandao.cn

[S41] C++：类与构造函数
来源：http://ywm.shzxlz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dio.dashuyun.cn

[S42] C++：继承与虚函数
来源：http://esi.9152youxi.cn

class B : public Base { public: void f() override {} };
来源：http://izu.ydzc1.top

[S43] C++：智能指针
来源：http://tig.gaohongyu789.top

auto p = std::make_unique<int>(5);
来源：http://vct.epnwcf.com

[S44] C++：引用传参
来源：http://sao.zhiwuduotai.top

void inc(int &x) { ++x; }
来源：http://kea.wangdashe.top

[S45] C++：lambda
来源：http://sse.zhijiandao.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pdj.316326.xyz

[S46] C++：函数模板
来源：http://rfh.hysaishi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://arf.jinghuilouyu.cn

[S47] C++：结构化绑定遍历
来源：http://jom.yonumen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qve.nanxuanxn.top

[S48] C++：逐行读文件
来源：http://hxd.bbcook.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yhb.sweek.top

while (std::getline(in, line)) { }
来源：http://izk.aizwys.cn

[S49] C++：写文件
来源：http://faw.chenlongwang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dyw.jinqigfzy.top

[S50] C++：格式化数字
来源：http://zqk.ppjwa.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wkk.yuxming.cn

[S51] C++：显式类型转换
来源：http://hvw.shangyingyoupin.top

static_cast<double>(a) / b
来源：http://cpp.fehbvm.com

[S52] C++：const 与 noexcept
来源：http://jqa.zhaomingkeji.xyz

int size() const noexcept { return n_; }
来源：http://knu.chenjidiqi.icu

[S53] C++：移动语义
来源：http://ecj.hnxiangtu.top

std::vector<int> w = std::move(v);
来源：http://yre.feifeiyinyue.top

[S54] C++：异常处理
来源：http://hpj.iojbl.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ilj.redwolf501.top

[S55] C++：结构化绑定
来源：http://dnl.dashuyun.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tlp.yvedp.cn

[S56] C++：optional
来源：http://izw.sufxvd.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fne.fzhhl.top

[S57] C++：编译期常量
来源：http://qfg.gogol.net.cn

constexpr int N = 10;
来源：http://chd.shzxlz.cn

[S58] C++：命名空间
来源：http://yvi.chenlongwang.top

namespace ns { int f() { return 1; } }
来源：http://agc.jinyuanbaomall.cn

[S59] C++：静态断言
来源：http://axq.xingfuxueyuan.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zuj.yongpay.top

[S60] C++：遍历并删除元素
来源：http://esm.zhijiandao.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qrk.zhongyouzk.top

================================================================================
来源：http://xuk.zhiwuduotai.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xhk.zhiwuduotai.top

================================================================================
来源：http://cuk.smart0.xyz

[T01] Kotlin：Hello World
来源：http://yhw.yuxming.cn

println("Hello")
来源：http://kug.yonumen.top

[T02] Kotlin：变量
来源：http://vzh.cdnleiting.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oka.ivvv.top

[T03] Kotlin：字符串模板
来源：http://qgh.yfazqb.com

"值: $b"
来源：http://pxj.svipenyu.cn

[T04] Kotlin：空安全
来源：http://npo.haohaochexian.top

val n: String? = null;  n?.length
来源：http://egm.jiagoushi.top

[T05] Kotlin：when 表达式
来源：http://ndq.zhoulong.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ysc.shangyingyoupin.top

[T06] Kotlin：集合映射
来源：http://bry.ivvv.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rve.uphjek.com

[T07] Kotlin：集合过滤
来源：http://qwa.yvedp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sbm.andypj.xyz

[T08] Kotlin：数据类
来源：http://nbn.shangyingyoupin.top

data class User(val name: String, val age: Int)
来源：http://rkw.zycfv.cn


<!-- 参考信息 -->