代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ngn.zdqjudy.top

[R08] 数值比较
来源：http://ayd.epnwcf.com

if (( a > b )); then echo "a 更大"; fi
来源：http://zma.tianlin.xyz

[R09] 字符串比较
来源：http://ojm.smart0.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rby.cdnleiting.top

[R10] 正则匹配
来源：http://foq.zhengqikj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wkq.zhiwuduotai.top

[R11] case 多分支
来源：http://oib.jinqigufen.top

case "$1" in
来源：http://lbq.316326.xyz

start) echo "启动" ;;
来源：http://spb.tarul.cn

stop)  echo "停止" ;;
来源：http://fnk.shzxlz.cn

*)     echo "未知命令" ;;
来源：http://efz.aibaodan.cn

esac
来源：http://lyi.daria6918.cn

[R12] for 遍历文件
来源：http://lld.sufxvd.cn

for f in *.txt; do echo "$f"; done
来源：http://mnu.zhoulong.xyz

[R13] for 计数循环
来源：http://tcl.shzxlz.cn

for i in {1..10}; do echo "$i"; done
来源：http://aos.yuanzhike.top

[R14] C 风格 for
来源：http://vrv.zhixingplan.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hbl.shanyushiyangkeji.top

[R15] while 逐行读文件
来源：http://ubd.vqdsnc.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://udy.hammf.cn

[R16] until 等待条件
来源：http://kfz.ydzc1.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bqp.aibaodan.cn

[R17] 数组定义与取值
来源：http://wnc.yj202588.top

arr=(a b c); echo "${arr[0]}"
来源：http://lmj.fanxiaobao.xyz

[R18] 遍历数组
来源：http://spo.sysykeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dcw.fktsv.cn

[R19] 数组长度
来源：http://blr.iojbl.cn

echo "${#arr[@]}"
来源：http://rig.yuxming.cn

[R20] 关联数组（字典）
来源：http://yaa.tianlin.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wxo.fengsongda.top

[R21] 字符串长度
来源：http://ajq.mhx1999.top

echo "${#s}"
来源：http://cas.yanxiufei.cn

[R22] 截取子串
来源：http://yri.c1oappe.top

echo "${s:0:5}"
来源：http://kjn.jiagoushi.top

[R23] 字符串替换
来源：http://gbc.yj20258.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wza.hesvh.cn

[R24] 大小写转换
来源：http://bns.aibaodan.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fjx.hammf.cn

[R25] 去后缀 / 去前缀
来源：http://pwj.zhoulong.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://rqa.yuxming.cn

[R26] 命令替换
来源：http://jvl.shzxlz.cn

now=$(date +%F); echo "$now"
来源：http://xcu.dashuyun.cn

[R27] 算术展开
来源：http://cip.zhengqikj.top

echo $((1 + 2 * 3))
来源：http://ije.yj20258888.top

[R28] 浮点运算
来源：http://yaa.shzxlz.cn

echo "scale=2; 10/3" | bc
来源：http://olp.pycfn.com

[R29] 定义函数
来源：http://elj.aibaodan.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://aux.gogol.net.cn

[R30] 函数返回状态码
来源：http://tev.hfpthk.cn

f() { return 0; }; f || echo "失败了"
来源：http://eei.yj202588.top

[R31] 局部变量
来源：http://nmk.cheryme.top

f() { local x=1; echo "$x"; }
来源：http://pmf.jqgufenzy.top

[R32] 参数个数校验
来源：http://isl.wangdashe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dsb.hcnkem.com

[R33] 捕获错误并提示行号
来源：http://stw.sjlbkw.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fot.0kj1m.cn

[R34] 退出时清理
来源：http://dbt.andypj.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://mkr.chenjidiqi.icu

[R35] 后台执行并等待
来源：http://cbj.cheryme.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zng.ydjk.org.cn

[R36] 并发执行多个任务
来源：http://kvb.jqgufenzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ana.shanyushiyangtech.top

[R37] 把输出赋给变量
来源：http://wfc.jinqigufen.top

files=$(ls -1)
来源：http://yyn.pycfn.com

[R38] 管道串联
来源：http://wyt.vehdjk.com

cat a.txt | grep -i error | wc -l
来源：http://drf.fanxiaobao.xyz

[R39] 重定向标准输出与错误
来源：http://dev.vehdjk.com

cmd > out.log 2>&1
来源：http://jpp.jinqigfzy.top

[R40] 追加写日志
来源：http://uog.shanyushiyangtech.top

echo "log" >> out.log
来源：http://hdw.zdqjudy.top

[R41] 丢弃输出
来源：http://max.andypj.xyz

cmd >/dev/null 2>&1
来源：http://ajf.xuanzx.com

[R42] 输入重定向
来源：http://tyz.zhengqikj.top

wc -l < a.txt
来源：http://dmc.hcnkem.com

[R43] 按名字查找文件
来源：http://auf.daria6918.cn

find . -name "*.log" -type f
来源：http://zvv.jinqigfzy.top

[R44] 按修改时间查找
来源：http://jho.wangdashe.top

find . -mtime -7 -type f
来源：http://lyz.zhaomingkeji.xyz

[R45] 批量删除
来源：http://zxm.hnxiangtu.top

find . -name "*.tmp" -delete
来源：http://sej.guannengcc.top

[R46] 递归替换文件内容
来源：http://tlv.wangdashe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nck.wangdashe.top

[R47] sed 单行替换
来源：http://gbm.xingfuxueyuan.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://qzy.daxiang520.top

[R48] awk 取指定列
来源：http://iaa.cucudq.cn

awk '{print $1, $3}' a.txt
来源：http://vjb.hnqzz.top

[R49] awk 带条件
来源：http://snm.cucudq.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yyy.jinyuanbaomall.cn

[R50] awk 求和
来源：http://wce.shanyushiyangtech.top

awk '{s += $2} END {print s}' a.txt
来源：http://fam.yonumen.top

[R51] 排序去重取前几
来源：http://guj.shanyushiyangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://doj.tianlin.xyz

[R52] 统计行数
来源：http://oxy.hnqzz.top

wc -l a.txt
来源：http://khr.hongshengwenyu.top

[R53] 查看文件头与实时尾
来源：http://ont.hnqzz.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nto.yangfankeji.com

[R54] 比较两个文件
来源：http://ynl.nwbrower.top

diff a.txt b.txt
来源：http://jtb.tian-w.cn

[R55] 压缩与解压
来源：http://kcf.xuetiantiany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zhr.ehwqpu.com

[R56] 远程拷贝
来源：http://usl.fengsongda.top

scp file user@host:/path/
来源：http://yzj.316326.xyz

[R57] 远程执行命令
来源：http://lde.zhixingplan.top

ssh user@host 'uptime'
来源：http://oaa.chenlongwang.top

[R58] 下载文件
来源：http://kvh.gzhubu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wld.yvedp.cn

[R59] 发 POST JSON
来源：http://pah.aizwys.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ijm.shangyingyoupin.top

[R60] 只看 HTTP 状态码
来源：http://isf.zhongyouzk.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ydi.shanyushiyangkeji.top

[R61] 磁盘占用
来源：http://owz.cashguo.top

df -h;  du -sh *
来源：http://vby.pycfn.com

[R62] 找最占空间的文件
来源：http://mih.svipenyu.cn

du -ah . | sort -rh | head -10
来源：http://bjc.tianlin.xyz

[R63] 内存与进程
来源：http://hkf.cqqwz.cn

free -h;  ps aux | grep nginx
来源：http://mda.nwbrower.top

[R64] 结束进程
来源：http://ylm.xinyue.icu

kill -9 $(pgrep -f app.py)
来源：http://zbd.jinyuanbaomall.cn

[R65] 查看端口占用
来源：http://phe.fanxiaobao.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kaj.vqdsnc.cn

[R66] 定时任务
来源：http://cvy.zhaomingkeji.xyz

crontab -e;  crontab -l
来源：http://ltc.shuidangran.top

[R67] 生成随机十六进制串
来源：http://nyh.jinqigfzy.top

openssl rand -hex 16
来源：http://chk.bjfxy.top

[R68] 计算文件校验值
来源：http://jxk.guannengcc.top

sha256sum a.txt;  md5sum a.txt
来源：http://uym.wangdashe.top

[R69] 生成随机密码
来源：http://wyv.zycfv.cn

head -c 16 /dev/urandom | base64
来源：http://yrl.iojbl.cn

[R70] 时间戳与互转
来源：http://wyb.birdmap.top

date +%s;  date -d @1700000000
来源：http://gto.cucudq.cn

[R71] 日期格式化
来源：http://hdk.xuetiantiany.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vfd.ydzc1.top

[R72] 等待端口就绪
来源：http://uul.ehwqpu.com

until nc -z localhost 3306; do sleep 1; done
来源：http://cci.zhixingplan.top

[R73] 分割大日志
来源：http://hum.sufxvd.cn

split -l 1000 big.log part_
来源：http://mje.jlsjyb.cn

[R74] 批量重命名
来源：http://wdr.vehdjk.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zce.nwbrower.top

[R75] 导出环境变量
来源：http://vma.iojbl.cn

export PATH="$HOME/bin:$PATH"
来源：http://yzk.guannengcc.top

[R76] 使用临时文件
来源：http://vht.xuanzx.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qcj.meibo888.top

[R77] 读取用户输入
来源：http://pja.nwbrower.top

read -rp "请输入: " ans
来源：http://ums.zdqjudy.top

[R78] 交互式菜单
来源：http://syq.zhongyouzk.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tyc.ydjk.org.cn

[R79] 解析命令行选项
来源：http://gnk.gotoacloud.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://prb.ehwqpu.com

[R80] 查看脚本执行耗时
来源：http://mxf.mhx1999.top

time ./run.sh
来源：http://who.gzhubu.top

================================================================================
来源：http://bbm.fktsv.cn

S. C / C++ 专题
来源：http://bjg.xinyue.icu

================================================================================
来源：http://rvq.yongpay.top

[S01] C：Hello World
来源：http://onv.0kj1m.cn

#include <stdio.h>
来源：http://ryz.aibaodan.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mqo.hesvh.cn

[S02] C：变量与格式化输出
来源：http://gch.havefunace.top

int a = 10; printf("%d\n", a);
来源：http://dum.zhaomingkeji.xyz

[S03] C：读入整数
来源：http://oan.quarkkingdee.top

int x; scanf("%d", &x);
来源：http://rzz.havefunace.top

[S04] C：字符串复制
来源：http://rtq.shanyushiyangtech.top

char dst[32]; strcpy(dst, "hi");
来源：http://dfi.jlsjyb.cn

[S05] C：字符串长度
来源：http://fqn.ybcxt.top

strlen(s)
来源：http://hfz.yuanzhike.top

[S06] C：字符串比较
来源：http://wjh.hcnkem.com

strcmp(a, b) == 0
来源：http://qhu.dianchejie.cn

[S07] C：数组遍历求和
来源：http://sww.guannengcc.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://urg.chenjidiqi.icu

[S08] C：动态内存分配与释放
来源：http://olm.jinqigufen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eeq.ehwqpu.com

[S09] C：结构体定义与初始化
来源：http://qil.jianghu66.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hhs.zhijiandao.cn

[S10] C：指针与解引用
来源：http://ujy.jyoumei.cn

int *p = &a;  *p = 5;
来源：http://mjg.chenlongwang.top

[S11] C：逐行读文件
来源：http://fid.yonumen.top

FILE *f = fopen("a.txt", "r");
来源：http://vug.daxiang520.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://gjg.zhoulong.xyz

fclose(f);
来源：http://nyo.cashguo.top

[S12] C：写文件
来源：http://obd.vqdsnc.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://msu.chenjidiqi.icu

[S13] C：宏定义
来源：http://jdf.gotoacloud.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tpw.andypj.xyz

[S14] C：枚举
来源：http://cod.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://rww.dianchejie.cn

[S15] C：类型转换
来源：http://yho.sweek.top

(double) a / b
来源：http://yva.jinyuanbaomall.cn

[S16] C：位操作置位
来源：http://vqh.guannengcc.top

x |= (1 << 3);
来源：http://jnq.zhaomingkeji.xyz

[S17] C：安全拼接字符串
来源：http://gvv.wangshuangyany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mvp.gogol.net.cn

[S18] C：命令行参数
来源：http://ugj.shangyingyoupin.top

int main(int argc, char **argv)
来源：http://rro.vehdjk.com

[S19] C：快速排序
来源：http://afk.zdbjq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ati.shuidangran.top

[S20] C：二分查找
来源：http://hee.sysykeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mrw.zhijiandao.cn

[S21] C：字符类别判断
来源：http://mnu.dianchejie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wvy.jlsjyb.cn

[S22] C：字符串转数字
来源：http://jjc.snrcjt.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cqd.hammf.cn

[S23] C：随机数
来源：http://osk.jianghu66.top

srand(time(NULL));  int r = rand() % 100;
来源：http://voz.quarkkingdee.top

[S24] C：获取本地时间
来源：http://lkt.mhx1999.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qnu.vqdsnc.cn

[S25] C：内存拷贝
来源：http://edf.jinyuanbaomall.cn

memcpy(dst, src, n);
来源：http://dwt.havefunace.top

[S26] C：内存清零
来源：http://cgc.gzhubu.top

memset(a, 0, sizeof a);
来源：http://wvd.sxryk.cn

[S27] C：定义常量
来源：http://gbr.jinqigufen.top

const double PI = 3.14159;
来源：http://wir.vehdjk.com

[S28] C：静态变量
来源：http://dum.yvedp.cn

static int counter = 0;
来源：http://vue.bjfxy.top

[S29] C：变参函数
来源：http://upu.shanyushiyangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rqx.jiagoushi.top

[S30] C：头文件保护
来源：http://wce.hfpthk.cn

#ifndef X_H
来源：http://fud.fanxiaobao.xyz

#define X_H
来源：http://vwu.yanxiufei.cn

#endif
来源：http://lwt.dianchejie.cn

[S31] C++：Hello World
来源：http://yif.ywan-chungtsiang.top

#include <iostream>
来源：http://hhu.zhoulong.xyz

int main() { std::cout << "Hello\n"; }
来源：http://kqb.zycfv.cn

[S32] C++：字符串
来源：http://rdc.svipenyu.cn

std::string s = "hi";  s += "!";
来源：http://rqk.yueranfly.top

[S33] C++：vector 增删
来源：http://duo.epnwcf.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lky.yongpay.top

[S34] C++：遍历 vector
来源：http://srb.bjfxy.top

for (auto &x : v) { std::cout << x; }
来源：http://ztw.dashuyun.cn

[S35] C++：map
来源：http://zcw.ydzc1.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zrg.gotoacloud.top

[S36] C++：unordered_map
来源：http://rfu.zdbjq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ifx.bjfxy.top

[S37] C++：set
来源：http://fsz.daria6918.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://irm.redwolf501.top

[S38] C++：排序
来源：http://xtc.aibaodan.cn

std::sort(v.begin(), v.end());
来源：http://mor.feifeiyinyue.top

[S39] C++：自定义比较器排序
来源：http://uwo.yuxming.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wsy.hcnkem.com

[S40] C++：查找元素
来源：http://xwc.smart0.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qpc.ctjpmb.com

[S41] C++：类与构造函数
来源：http://msq.xingfuxueyuan.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rqq.hammf.cn

[S42] C++：继承与虚函数
来源：http://rhh.gogol.net.cn

class B : public Base { public: void f() override {} };
来源：http://amw.jqgufenzy.top

[S43] C++：智能指针
来源：http://let.yonumen.top

auto p = std::make_unique<int>(5);
来源：http://ueh.jinqigfzy.top

[S44] C++：引用传参
来源：http://ilo.hesvh.cn

void inc(int &x) { ++x; }
来源：http://ahr.kuanghao11.cn

[S45] C++：lambda
来源：http://yej.yuanzhike.top

auto add = [](int a, int b) { return a + b; };
来源：http://bdn.hcnkem.com

[S46] C++：函数模板
来源：http://gse.xziqi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://amy.tianlin.xyz

[S47] C++：结构化绑定遍历
来源：http://fqo.cashguo.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ueh.chenzaomai.com

[S48] C++：逐行读文件
来源：http://jjt.bbcook.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jsi.xziqi.cn

while (std::getline(in, line)) { }
来源：http://bxk.vqdsnc.cn

[S49] C++：写文件
来源：http://som.vehdjk.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eqb.hnxiangtu.top

[S50] C++：格式化数字
来源：http://sbq.meibo888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hsm.fehbvm.com

[S51] C++：显式类型转换
来源：http://xjj.cqqwz.cn

static_cast<double>(a) / b
来源：http://yka.cucudq.cn

[S52] C++：const 与 noexcept
来源：http://pjb.pengpengdd.cyou

int size() const noexcept { return n_; }
来源：http://xfh.fehbvm.com

[S53] C++：移动语义
来源：http://kqx.tanke756.top

std::vector<int> w = std::move(v);
来源：http://ppp.yueranfly.top

[S54] C++：异常处理
来源：http://lkj.zhengqikj.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://roy.sxryk.cn

[S55] C++：结构化绑定
来源：http://xfn.ivvv.top

auto [a, b] = std::make_pair(1, 2);
来源：http://yji.haohaochexian.top

[S56] C++：optional
来源：http://zje.cucudq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sjf.fengsongda.top

[S57] C++：编译期常量
来源：http://shf.ivvv.top

constexpr int N = 10;
来源：http://yce.sweek.top

[S58] C++：命名空间
来源：http://yvb.cqqwz.cn

namespace ns { int f() { return 1; } }
来源：http://mme.zhongyouzk.top

[S59] C++：静态断言
来源：http://yzb.jinghuilouyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gmx.iojbl.cn

[S60] C++：遍历并删除元素
来源：http://hru.cqqwz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ufr.ywan-chungtsiang.top

================================================================================
来源：http://ljg.316326.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oht.chenzaomai.com

================================================================================
来源：http://age.pengpengdd.cyou

[T01] Kotlin：Hello World
来源：http://jea.aibaodan.cn

println("Hello")
来源：http://mny.fktsv.cn

[T02] Kotlin：变量
来源：http://ayn.bbcook.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qyo.yueranfly.top

[T03] Kotlin：字符串模板
来源：http://yfe.tian-w.cn

"值: $b"
来源：http://mzt.fehbvm.com

[T04] Kotlin：空安全
来源：http://xbm.yuxming.cn

val n: String? = null;  n?.length
来源：http://btg.xingfuxueyuan.xyz

[T05] Kotlin：when 表达式
来源：http://afc.bjfxy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dds.sysykeji.top

[T06] Kotlin：集合映射
来源：http://blc.zhongyouzk.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hfu.c1oappe.top

[T07] Kotlin：集合过滤
来源：http://ddr.smart0.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://opw.zhijiandao.cn

[T08] Kotlin：数据类
来源：http://rpv.kuanghao11.cn

data class User(val name: String, val age: Int)
来源：http://hng.bbcook.cn


<!-- 参考信息 -->