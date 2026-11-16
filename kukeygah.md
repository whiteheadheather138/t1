代发 wailian999

name="${1:-default}"
来源：http://cno.xingfuxueyuan.xyz

[R06] 判断命令是否存在
来源：http://gjq.zhengqikj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cqr.uphjek.com

[R07] if 判断文件
来源：http://ztz.zhixingplan.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gmv.iojbl.cn

[R08] 数值比较
来源：http://fdd.uphjek.com

if (( a > b )); then echo "a 更大"; fi
来源：http://wsm.0kj1m.cn

[R09] 字符串比较
来源：http://rfb.yj202588.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://khq.guannengcc.top

[R10] 正则匹配
来源：http://cfq.tianlin.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uot.vqdsnc.cn

[R11] case 多分支
来源：http://zsy.iojbl.cn

case "$1" in
来源：http://kir.ehwqpu.com

start) echo "启动" ;;
来源：http://tlr.zycfv.cn

stop)  echo "停止" ;;
来源：http://osy.ydjk.org.cn

*)     echo "未知命令" ;;
来源：http://kpq.hnxiangtu.top

esac
来源：http://exu.fanxiaobao.xyz

[R12] for 遍历文件
来源：http://bln.hfpthk.cn

for f in *.txt; do echo "$f"; done
来源：http://ale.chenlongwang.top

[R13] for 计数循环
来源：http://bsp.fengsongda.top

for i in {1..10}; do echo "$i"; done
来源：http://bxt.redwolf501.top

[R14] C 风格 for
来源：http://hyb.pycfn.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kjw.pengpengdd.cyou

[R15] while 逐行读文件
来源：http://moh.yj20258888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bqp.gzhubu.top

[R16] until 等待条件
来源：http://vuo.gzhubu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dqk.9152youxi.cn

[R17] 数组定义与取值
来源：http://wrc.yvedp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hor.yuanzhike.top

[R18] 遍历数组
来源：http://gth.sweek.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://thr.yanxiufei.cn

[R19] 数组长度
来源：http://iqq.fehbvm.com

echo "${#arr[@]}"
来源：http://nwq.redwolf501.top

[R20] 关联数组（字典）
来源：http://log.xuanzx.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yyf.ehwqpu.com

[R21] 字符串长度
来源：http://kug.zycfv.cn

echo "${#s}"
来源：http://tjd.uphjek.com

[R22] 截取子串
来源：http://hqa.tian-w.cn

echo "${s:0:5}"
来源：http://dpw.wangdashe.top

[R23] 字符串替换
来源：http://onq.meibo888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bsr.zhengqikj.top

[R24] 大小写转换
来源：http://rih.jinyuanbaomall.cn

echo "${s^^}"; echo "${s,,}"
来源：http://djf.cucudq.cn

[R25] 去后缀 / 去前缀
来源：http://lkd.jinqigfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://tjo.xziqi.cn

[R26] 命令替换
来源：http://nhr.chenjidiqi.icu

now=$(date +%F); echo "$now"
来源：http://dsy.yfazqb.com

[R27] 算术展开
来源：http://vyt.cashguo.top

echo $((1 + 2 * 3))
来源：http://owf.shzxlz.cn

[R28] 浮点运算
来源：http://bwh.yj202588.top

echo "scale=2; 10/3" | bc
来源：http://wvh.xinyue.icu

[R29] 定义函数
来源：http://phs.guannengcc.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ity.jinqigufen.top

[R30] 函数返回状态码
来源：http://vqq.zhiwuduotai.top

f() { return 0; }; f || echo "失败了"
来源：http://rsx.jqgufenzy.top

[R31] 局部变量
来源：http://xxe.fanxiaobao.xyz

f() { local x=1; echo "$x"; }
来源：http://cyy.gaohongyu789.top

[R32] 参数个数校验
来源：http://lyq.shuidangran.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vod.jyoumei.cn

[R33] 捕获错误并提示行号
来源：http://qwm.ywan-chungtsiang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nbs.kuanghao11.cn

[R34] 退出时清理
来源：http://ztt.hnxiangtu.top

trap 'rm -f "$tmp"' EXIT
来源：http://mya.sufxvd.cn

[R35] 后台执行并等待
来源：http://ekp.dianchejie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vhu.yuanzhike.top

[R36] 并发执行多个任务
来源：http://xbb.jqgfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://znz.ehwqpu.com

[R37] 把输出赋给变量
来源：http://bhj.zhiwuduotai.top

files=$(ls -1)
来源：http://ayg.dianchejie.cn

[R38] 管道串联
来源：http://bfp.mhx1999.top

cat a.txt | grep -i error | wc -l
来源：http://har.jyoumei.cn

[R39] 重定向标准输出与错误
来源：http://mjt.jinqigufen.top

cmd > out.log 2>&1
来源：http://sdo.xingfuxueyuan.xyz

[R40] 追加写日志
来源：http://tfh.quarkkingdee.top

echo "log" >> out.log
来源：http://jwa.sweek.top

[R41] 丢弃输出
来源：http://qgi.zhixingplan.top

cmd >/dev/null 2>&1
来源：http://mrm.dashuyun.cn

[R42] 输入重定向
来源：http://zcu.xuanzx.com

wc -l < a.txt
来源：http://htb.fktsv.cn

[R43] 按名字查找文件
来源：http://vmu.xuetiantiany.cn

find . -name "*.log" -type f
来源：http://jcp.tarul.cn

[R44] 按修改时间查找
来源：http://lwy.jlsjyb.cn

find . -mtime -7 -type f
来源：http://tls.yj20258888.top

[R45] 批量删除
来源：http://iqg.gotoacloud.top

find . -name "*.tmp" -delete
来源：http://ajs.tarul.cn

[R46] 递归替换文件内容
来源：http://mpa.pengpengdd.cyou

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uvr.sufxvd.cn

[R47] sed 单行替换
来源：http://emv.yanxiufei.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ggb.9152youxi.cn

[R48] awk 取指定列
来源：http://sjf.tarul.cn

awk '{print $1, $3}' a.txt
来源：http://tpt.shuidangran.top

[R49] awk 带条件
来源：http://yty.jinyuanbaomall.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cqk.xylfe.cn

[R50] awk 求和
来源：http://npx.ehwqpu.com

awk '{s += $2} END {print s}' a.txt
来源：http://lhx.gzhubu.top

[R51] 排序去重取前几
来源：http://gaw.xuanzx.com

sort a.txt | uniq -c | sort -rn | head
来源：http://yff.0kj1m.cn

[R52] 统计行数
来源：http://aua.vehdjk.com

wc -l a.txt
来源：http://seg.hywenlv.cn

[R53] 查看文件头与实时尾
来源：http://qki.fengsongda.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://whx.tanke756.top

[R54] 比较两个文件
来源：http://sdb.zhijiandao.cn

diff a.txt b.txt
来源：http://loc.zdqjudy.top

[R55] 压缩与解压
来源：http://cbk.aibaodan.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dpy.yanxiufei.cn

[R56] 远程拷贝
来源：http://emu.hongshengwenyu.top

scp file user@host:/path/
来源：http://bvj.guowangkeji.top

[R57] 远程执行命令
来源：http://jqm.fehbvm.com

ssh user@host 'uptime'
来源：http://rak.mhx1999.top

[R58] 下载文件
来源：http://acu.guannengcc.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uwz.haohaochexian.top

[R59] 发 POST JSON
来源：http://dsb.shuidangran.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qeg.xinyue.icu

[R60] 只看 HTTP 状态码
来源：http://zzq.epnwcf.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qmk.pengpengdd.cyou

[R61] 磁盘占用
来源：http://lnu.9152youxi.cn

df -h;  du -sh *
来源：http://oyh.aibaodan.cn

[R62] 找最占空间的文件
来源：http://xrk.jiagoushi.top

du -ah . | sort -rh | head -10
来源：http://jsw.bjfxy.top

[R63] 内存与进程
来源：http://jdh.shanyushiyangkeji.top

free -h;  ps aux | grep nginx
来源：http://jis.shangyingyoupin.top

[R64] 结束进程
来源：http://utt.zhengqikj.top

kill -9 $(pgrep -f app.py)
来源：http://gpt.bbcook.cn

[R65] 查看端口占用
来源：http://fcz.ctjpmb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ont.tarul.cn

[R66] 定时任务
来源：http://qxv.wangdashe.top

crontab -e;  crontab -l
来源：http://aza.zhaomingkeji.xyz

[R67] 生成随机十六进制串
来源：http://ygx.c1oappe.top

openssl rand -hex 16
来源：http://ntt.hcnkem.com

[R68] 计算文件校验值
来源：http://irg.316326.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://zic.yfazqb.com

[R69] 生成随机密码
来源：http://lpk.haohaochexian.top

head -c 16 /dev/urandom | base64
来源：http://lxy.sjlbkw.cn

[R70] 时间戳与互转
来源：http://ctf.gogol.net.cn

date +%s;  date -d @1700000000
来源：http://ami.zhongyouzk.top

[R71] 日期格式化
来源：http://mib.ydjk.org.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vbe.fktsv.cn

[R72] 等待端口就绪
来源：http://fta.xuetiantiany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cvx.ybcxt.top

[R73] 分割大日志
来源：http://gnk.wangdashe.top

split -l 1000 big.log part_
来源：http://xkt.nanxinkj.top

[R74] 批量重命名
来源：http://kpw.dashuyun.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://chm.hammf.cn

[R75] 导出环境变量
来源：http://zha.snrcjt.cn

export PATH="$HOME/bin:$PATH"
来源：http://mwl.svipenyu.cn

[R76] 使用临时文件
来源：http://ddm.vqdsnc.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nuz.hongshengwenyu.top

[R77] 读取用户输入
来源：http://jhj.cucudq.cn

read -rp "请输入: " ans
来源：http://paw.ydjk.org.cn

[R78] 交互式菜单
来源：http://vjl.feifeiyinyue.top

select opt in a b c; do echo "$opt"; break; done
来源：http://yjh.chenlongwang.top

[R79] 解析命令行选项
来源：http://pjq.fktsv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://twu.fehbvm.com

[R80] 查看脚本执行耗时
来源：http://mdz.gotoacloud.top

time ./run.sh
来源：http://lnt.hywenlv.cn

================================================================================
来源：http://mau.haohaochexian.top

S. C / C++ 专题
来源：http://qgh.zdqjudy.top

================================================================================
来源：http://zln.nwbrower.top

[S01] C：Hello World
来源：http://ydt.jianghu66.top

#include <stdio.h>
来源：http://mzb.feifeiyinyue.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ahn.c1oappe.top

[S02] C：变量与格式化输出
来源：http://gqj.gotoacloud.top

int a = 10; printf("%d\n", a);
来源：http://veb.yj20258888.top

[S03] C：读入整数
来源：http://qfe.ivvv.top

int x; scanf("%d", &x);
来源：http://pwl.zycfv.cn

[S04] C：字符串复制
来源：http://usk.jiagoushi.top

char dst[32]; strcpy(dst, "hi");
来源：http://fiu.havefunace.top

[S05] C：字符串长度
来源：http://mdk.shangyingyoupin.top

strlen(s)
来源：http://kvv.ybcxt.top

[S06] C：字符串比较
来源：http://cpd.hnxiangtu.top

strcmp(a, b) == 0
来源：http://cqq.ydzc1.top

[S07] C：数组遍历求和
来源：http://hhq.snrcjt.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gzp.zhixingplan.top

[S08] C：动态内存分配与释放
来源：http://ggc.9152youxi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ayt.haohaochexian.top

[S09] C：结构体定义与初始化
来源：http://wmc.yuxming.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wbi.tanke756.top

[S10] C：指针与解引用
来源：http://vsp.tianlin.xyz

int *p = &a;  *p = 5;
来源：http://jxy.chenjidiqi.icu

[S11] C：逐行读文件
来源：http://jvn.tanke756.top

FILE *f = fopen("a.txt", "r");
来源：http://bnc.birdmap.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://slx.sysykeji.top

fclose(f);
来源：http://xqj.bbcook.cn

[S12] C：写文件
来源：http://ezu.aizwys.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pgj.xylfe.cn

[S13] C：宏定义
来源：http://xgt.redwolf501.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tiu.yj20258.top

[S14] C：枚举
来源：http://yil.daxiang520.top

enum Color { RED, GREEN, BLUE };
来源：http://pzl.smart0.xyz

[S15] C：类型转换
来源：http://xic.sufxvd.cn

(double) a / b
来源：http://mjx.zhongyouzk.top

[S16] C：位操作置位
来源：http://ulp.chenjidiqi.icu

x |= (1 << 3);
来源：http://asv.yanxiufei.cn

[S17] C：安全拼接字符串
来源：http://eqv.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eky.chenzaomai.com

[S18] C：命令行参数
来源：http://gfv.sweek.top

int main(int argc, char **argv)
来源：http://mza.gotoacloud.top

[S19] C：快速排序
来源：http://jqi.yanxiufei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sjz.fengsongda.top

[S20] C：二分查找
来源：http://wox.pycfn.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://shr.nanxuanxn.top

[S21] C：字符类别判断
来源：http://drv.sweek.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://twg.redwolf501.top

[S22] C：字符串转数字
来源：http://lyo.hongshengwenyu.top

atoi("42");  strtod("3.14", NULL);
来源：http://qkc.sweek.top

[S23] C：随机数
来源：http://kte.fanxiaobao.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://snb.fanxiaobao.xyz

[S24] C：获取本地时间
来源：http://xcz.cheryme.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xuj.svipenyu.cn

[S25] C：内存拷贝
来源：http://ilo.jqgufenzy.top

memcpy(dst, src, n);
来源：http://lae.yfazqb.com

[S26] C：内存清零
来源：http://lev.sweek.top

memset(a, 0, sizeof a);
来源：http://hlb.wangshuangyany.cn

[S27] C：定义常量
来源：http://oet.9152youxi.cn

const double PI = 3.14159;
来源：http://kwk.svipenyu.cn

[S28] C：静态变量
来源：http://ymb.cqqwz.cn

static int counter = 0;
来源：http://qks.zhixingplan.top

[S29] C：变参函数
来源：http://zjr.xylfe.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zej.cucudq.cn

[S30] C：头文件保护
来源：http://jeo.andypj.xyz

#ifndef X_H
来源：http://ctw.yfazqb.com

#define X_H
来源：http://qvy.fehbvm.com

#endif
来源：http://mkv.shanyushiyangtech.top

[S31] C++：Hello World
来源：http://qma.shanyushiyangkeji.top

#include <iostream>
来源：http://agx.yonumen.top

int main() { std::cout << "Hello\n"; }
来源：http://eex.ppjwa.cn

[S32] C++：字符串
来源：http://clf.fzhhl.top

std::string s = "hi";  s += "!";
来源：http://pgr.havefunace.top

[S33] C++：vector 增删
来源：http://zxq.fzhhl.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yjf.316326.xyz

[S34] C++：遍历 vector
来源：http://oqq.jianghu66.top

for (auto &x : v) { std::cout << x; }
来源：http://dsl.hesvh.cn

[S35] C++：map
来源：http://pmt.zhiwuduotai.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yxk.havefunace.top

[S36] C++：unordered_map
来源：http://xel.c1oappe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://duo.dianchejie.cn

[S37] C++：set
来源：http://ouq.tarul.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vhy.zhongyouzk.top

[S38] C++：排序
来源：http://ron.shanyushiyangkeji.top

std::sort(v.begin(), v.end());
来源：http://zut.svipenyu.cn

[S39] C++：自定义比较器排序
来源：http://mvg.havefunace.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vwy.bbcook.cn

[S40] C++：查找元素
来源：http://ytp.ydjk.org.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pno.nwbrower.top

[S41] C++：类与构造函数
来源：http://idf.52xcode.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qwn.gzhubu.top

[S42] C++：继承与虚函数
来源：http://fog.wangshuangyany.cn

class B : public Base { public: void f() override {} };
来源：http://ubq.sweek.top

[S43] C++：智能指针
来源：http://lvc.yuxming.cn

auto p = std::make_unique<int>(5);
来源：http://apg.meibo888.top

[S44] C++：引用传参
来源：http://oze.zhengqikj.top

void inc(int &x) { ++x; }
来源：http://cqv.gogol.net.cn

[S45] C++：lambda
来源：http://cjb.mhx1999.top

auto add = [](int a, int b) { return a + b; };
来源：http://cyc.zhijiandao.cn

[S46] C++：函数模板
来源：http://bsx.316326.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qfg.hnxiangtu.top

[S47] C++：结构化绑定遍历
来源：http://nlo.shanyushiyangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bop.aibaodan.cn

[S48] C++：逐行读文件
来源：http://npb.xuanzx.com

std::ifstream in("a.txt");  std::string line;
来源：http://gwi.yj202588.top

while (std::getline(in, line)) { }
来源：http://say.sysykeji.top

[S49] C++：写文件
来源：http://fxo.haohaochexian.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://neu.wangshuangyany.cn

[S50] C++：格式化数字
来源：http://ume.yj20258888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ugx.nanxuanxn.top

[S51] C++：显式类型转换
来源：http://vog.hammf.cn

static_cast<double>(a) / b
来源：http://erh.jinyuanbaomall.cn

[S52] C++：const 与 noexcept
来源：http://szi.yueranfly.top

int size() const noexcept { return n_; }
来源：http://swb.yonumen.top

[S53] C++：移动语义
来源：http://pvc.birdmap.top

std::vector<int> w = std::move(v);
来源：http://zxz.zhaomingkeji.xyz

[S54] C++：异常处理
来源：http://ejk.haohaochexian.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qzp.gotoacloud.top

[S55] C++：结构化绑定
来源：http://pxl.sxryk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://eqs.yangfankeji.com

[S56] C++：optional
来源：http://axp.jqgufenzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lkq.9152youxi.cn

[S57] C++：编译期常量
来源：http://ffn.cqqwz.cn

constexpr int N = 10;
来源：http://dkh.pycfn.com

[S58] C++：命名空间
来源：http://ubr.cheryme.top

namespace ns { int f() { return 1; } }
来源：http://svs.ydzc1.top

[S59] C++：静态断言
来源：http://hff.fengsongda.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pcl.feifeiyinyue.top

[S60] C++：遍历并删除元素
来源：http://tgs.yj20258888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oxf.ydzc1.top

================================================================================
来源：http://qtd.hnqzz.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zvb.fehbvm.com

================================================================================
来源：http://gar.havefunace.top

[T01] Kotlin：Hello World
来源：http://rts.fktsv.cn

println("Hello")
来源：http://erj.yj20258888.top

[T02] Kotlin：变量
来源：http://kcg.0kj1m.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nzf.zhixingplan.top

[T03] Kotlin：字符串模板
来源：http://odn.zhongyouzk.top

"值: $b"
来源：http://crc.daria6918.cn

[T04] Kotlin：空安全
来源：http://luw.c1oappe.top

val n: String? = null;  n?.length
来源：http://pxb.gogol.net.cn

[T05] Kotlin：when 表达式
来源：http://mek.yangfankeji.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://che.yangfankeji.com

[T06] Kotlin：集合映射
来源：http://djn.jlsjyb.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jlu.shzxlz.cn


<!-- 参考信息 -->