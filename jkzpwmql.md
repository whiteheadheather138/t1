代发 wailian999

name="${1:-default}"
来源：http://cog.jinghuilouyu.cn

[R06] 判断命令是否存在
来源：http://zcc.jqgufenzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cgk.yuxming.cn

[R07] if 判断文件
来源：http://wpw.nanxuanxn.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uev.fehbvm.com

[R08] 数值比较
来源：http://jvw.svipenyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zln.hcnkem.com

[R09] 字符串比较
来源：http://hnc.pengpengdd.cyou

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kvk.meibo888.top

[R10] 正则匹配
来源：http://iob.cqqwz.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lqm.nwbrower.top

[R11] case 多分支
来源：http://yzu.hysaishi.cn

case "$1" in
来源：http://btz.zdqjudy.top

start) echo "启动" ;;
来源：http://njv.chenjidiqi.icu

stop)  echo "停止" ;;
来源：http://gxe.snrcjt.cn

*)     echo "未知命令" ;;
来源：http://fhx.feifeiyinyue.top

esac
来源：http://yqq.havefunace.top

[R12] for 遍历文件
来源：http://ykq.yuanzhike.top

for f in *.txt; do echo "$f"; done
来源：http://vfo.ywan-chungtsiang.top

[R13] for 计数循环
来源：http://kbx.bbcook.cn

for i in {1..10}; do echo "$i"; done
来源：http://xuf.yj202588.top

[R14] C 风格 for
来源：http://dcs.guannengcc.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cnd.uphjek.com

[R15] while 逐行读文件
来源：http://ugl.chenlongwang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rez.hongshengwenyu.top

[R16] until 等待条件
来源：http://nuv.xingfuxueyuan.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bmu.tianlin.xyz

[R17] 数组定义与取值
来源：http://agi.yanxiufei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://noh.haohaochexian.top

[R18] 遍历数组
来源：http://mvv.cashguo.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pjy.yfazqb.com

[R19] 数组长度
来源：http://muf.jqgfzy.top

echo "${#arr[@]}"
来源：http://pyl.birdmap.top

[R20] 关联数组（字典）
来源：http://dha.sweek.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://efy.havefunace.top

[R21] 字符串长度
来源：http://gil.cdnleiting.top

echo "${#s}"
来源：http://tzr.daria6918.cn

[R22] 截取子串
来源：http://owb.aibaodan.cn

echo "${s:0:5}"
来源：http://jdh.kuanghao11.cn

[R23] 字符串替换
来源：http://ozy.hysaishi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nmp.cashguo.top

[R24] 大小写转换
来源：http://vut.zhongyouzk.top

echo "${s^^}"; echo "${s,,}"
来源：http://lck.jinqigfzy.top

[R25] 去后缀 / 去前缀
来源：http://aoj.jinghuilouyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hgz.xingfuxueyuan.xyz

[R26] 命令替换
来源：http://xew.redwolf501.top

now=$(date +%F); echo "$now"
来源：http://ziw.shanyushiyangtech.top

[R27] 算术展开
来源：http://jqr.bbcook.cn

echo $((1 + 2 * 3))
来源：http://gam.gaohongyu789.top

[R28] 浮点运算
来源：http://ezf.c1oappe.top

echo "scale=2; 10/3" | bc
来源：http://lxl.zdbjq.cn

[R29] 定义函数
来源：http://dvi.yj20258.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fop.hywenlv.cn

[R30] 函数返回状态码
来源：http://vkr.vqdsnc.cn

f() { return 0; }; f || echo "失败了"
来源：http://ilz.birdmap.top

[R31] 局部变量
来源：http://rse.yangfankeji.com

f() { local x=1; echo "$x"; }
来源：http://kdr.meibo888.top

[R32] 参数个数校验
来源：http://dkx.uphjek.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://typ.ywan-chungtsiang.top

[R33] 捕获错误并提示行号
来源：http://xga.316326.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ptd.fktsv.cn

[R34] 退出时清理
来源：http://zuj.jinghuilouyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fhw.nanxuanxn.top

[R35] 后台执行并等待
来源：http://cnb.sysykeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hhd.hongshengwenyu.top

[R36] 并发执行多个任务
来源：http://geb.xingfuxueyuan.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jju.hammf.cn

[R37] 把输出赋给变量
来源：http://hgn.52xcode.cn

files=$(ls -1)
来源：http://ygv.bbcook.cn

[R38] 管道串联
来源：http://ryq.sufxvd.cn

cat a.txt | grep -i error | wc -l
来源：http://uxj.iojbl.cn

[R39] 重定向标准输出与错误
来源：http://nun.jinqigufen.top

cmd > out.log 2>&1
来源：http://uvf.zdbjq.cn

[R40] 追加写日志
来源：http://zso.gaohongyu789.top

echo "log" >> out.log
来源：http://chj.hnxiangtu.top

[R41] 丢弃输出
来源：http://zar.hysaishi.cn

cmd >/dev/null 2>&1
来源：http://nwb.shzxlz.cn

[R42] 输入重定向
来源：http://ugs.hywenlv.cn

wc -l < a.txt
来源：http://ruc.jinyuanbaomall.cn

[R43] 按名字查找文件
来源：http://zwx.chenlongwang.top

find . -name "*.log" -type f
来源：http://zqt.chenlongwang.top

[R44] 按修改时间查找
来源：http://fpw.sjlbkw.cn

find . -mtime -7 -type f
来源：http://owh.vehdjk.com

[R45] 批量删除
来源：http://gop.ivvv.top

find . -name "*.tmp" -delete
来源：http://xxi.guowangkeji.top

[R46] 递归替换文件内容
来源：http://iwq.jinqigufen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://enb.hnxiangtu.top

[R47] sed 单行替换
来源：http://mke.nanxinkj.top

sed -i 's/foo/bar/g' a.txt
来源：http://zzo.iojbl.cn

[R48] awk 取指定列
来源：http://ydi.tanke756.top

awk '{print $1, $3}' a.txt
来源：http://ifu.yuxming.cn

[R49] awk 带条件
来源：http://jrr.yonumen.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pst.tian-w.cn

[R50] awk 求和
来源：http://eyp.yueranfly.top

awk '{s += $2} END {print s}' a.txt
来源：http://uub.xuanzx.com

[R51] 排序去重取前几
来源：http://gxv.vqdsnc.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zlq.jianghu66.top

[R52] 统计行数
来源：http://svi.9152youxi.cn

wc -l a.txt
来源：http://asw.zycfv.cn

[R53] 查看文件头与实时尾
来源：http://hui.mhx1999.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vfu.meibo888.top

[R54] 比较两个文件
来源：http://zyw.jqgfzy.top

diff a.txt b.txt
来源：http://yyz.hfpthk.cn

[R55] 压缩与解压
来源：http://cna.feifeiyinyue.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://olt.sjlbkw.cn

[R56] 远程拷贝
来源：http://kmi.cucudq.cn

scp file user@host:/path/
来源：http://jqv.316326.xyz

[R57] 远程执行命令
来源：http://cet.xuanzx.com

ssh user@host 'uptime'
来源：http://xei.iojbl.cn

[R58] 下载文件
来源：http://bus.yonumen.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oaj.guowangkeji.top

[R59] 发 POST JSON
来源：http://uhs.shuidangran.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pou.hnqzz.top

[R60] 只看 HTTP 状态码
来源：http://okk.daxiang520.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zlf.jqgufenzy.top

[R61] 磁盘占用
来源：http://bwy.hnxiangtu.top

df -h;  du -sh *
来源：http://jui.shanyushiyangkeji.top

[R62] 找最占空间的文件
来源：http://axw.fengsongda.top

du -ah . | sort -rh | head -10
来源：http://jbf.svipenyu.cn

[R63] 内存与进程
来源：http://yra.jinqigufen.top

free -h;  ps aux | grep nginx
来源：http://cah.sweek.top

[R64] 结束进程
来源：http://ohv.fanxiaobao.xyz

kill -9 $(pgrep -f app.py)
来源：http://ite.jyoumei.cn

[R65] 查看端口占用
来源：http://xfa.jqgufenzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://muy.yfazqb.com

[R66] 定时任务
来源：http://gac.wangdashe.top

crontab -e;  crontab -l
来源：http://kav.0kj1m.cn

[R67] 生成随机十六进制串
来源：http://heg.hcnkem.com

openssl rand -hex 16
来源：http://mnp.gzhubu.top

[R68] 计算文件校验值
来源：http://eyp.meibo888.top

sha256sum a.txt;  md5sum a.txt
来源：http://kgr.guannengcc.top

[R69] 生成随机密码
来源：http://tim.epnwcf.com

head -c 16 /dev/urandom | base64
来源：http://sti.ctjpmb.com

[R70] 时间戳与互转
来源：http://hrf.hysaishi.cn

date +%s;  date -d @1700000000
来源：http://zcg.xinyue.icu

[R71] 日期格式化
来源：http://ial.dashuyun.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mbv.dashuyun.cn

[R72] 等待端口就绪
来源：http://cqy.pycfn.com

until nc -z localhost 3306; do sleep 1; done
来源：http://ryw.tanke756.top

[R73] 分割大日志
来源：http://ayn.nwbrower.top

split -l 1000 big.log part_
来源：http://pla.9152youxi.cn

[R74] 批量重命名
来源：http://dnl.ywan-chungtsiang.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wub.shuidangran.top

[R75] 导出环境变量
来源：http://vik.sweek.top

export PATH="$HOME/bin:$PATH"
来源：http://bih.pengpengdd.cyou

[R76] 使用临时文件
来源：http://jwh.bbcook.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pgp.sjlbkw.cn

[R77] 读取用户输入
来源：http://sts.redwolf501.top

read -rp "请输入: " ans
来源：http://jiv.yonumen.top

[R78] 交互式菜单
来源：http://nkv.yanxiufei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fmq.tian-w.cn

[R79] 解析命令行选项
来源：http://dho.haohaochexian.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ijc.xingfuxueyuan.xyz

[R80] 查看脚本执行耗时
来源：http://dfp.ydzc1.top

time ./run.sh
来源：http://ztw.shanyushiyangkeji.top

================================================================================
来源：http://zte.nwbrower.top

S. C / C++ 专题
来源：http://gav.hongshengwenyu.top

================================================================================
来源：http://kve.xuetiantiany.cn

[S01] C：Hello World
来源：http://lba.0kj1m.cn

#include <stdio.h>
来源：http://lez.tian-w.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://oep.sjlbkw.cn

[S02] C：变量与格式化输出
来源：http://vxc.jiagoushi.top

int a = 10; printf("%d\n", a);
来源：http://edh.guannengcc.top

[S03] C：读入整数
来源：http://njd.tanke756.top

int x; scanf("%d", &x);
来源：http://taj.shanyushiyangkeji.top

[S04] C：字符串复制
来源：http://jfo.yanxiufei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fxe.fktsv.cn

[S05] C：字符串长度
来源：http://gnb.xziqi.cn

strlen(s)
来源：http://qpb.xylfe.cn

[S06] C：字符串比较
来源：http://vhe.bjfxy.top

strcmp(a, b) == 0
来源：http://izq.snrcjt.cn

[S07] C：数组遍历求和
来源：http://xry.jqgufenzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bap.9152youxi.cn

[S08] C：动态内存分配与释放
来源：http://spu.xingfuxueyuan.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xxv.yanxiufei.cn

[S09] C：结构体定义与初始化
来源：http://xkq.sysykeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hfx.xuanzx.com

[S10] C：指针与解引用
来源：http://kyw.jinqigufen.top

int *p = &a;  *p = 5;
来源：http://rlx.smart0.xyz

[S11] C：逐行读文件
来源：http://uau.quarkkingdee.top

FILE *f = fopen("a.txt", "r");
来源：http://pbo.52xcode.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gze.sxryk.cn

fclose(f);
来源：http://etr.zhoulong.xyz

[S12] C：写文件
来源：http://seq.zdbjq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bcz.yj20258888.top

[S13] C：宏定义
来源：http://ass.hcnkem.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://juv.9152youxi.cn

[S14] C：枚举
来源：http://lrb.yonumen.top

enum Color { RED, GREEN, BLUE };
来源：http://hqq.jqgufenzy.top

[S15] C：类型转换
来源：http://bvj.jinqigufen.top

(double) a / b
来源：http://msb.jinqigufen.top

[S16] C：位操作置位
来源：http://umf.andypj.xyz

x |= (1 << 3);
来源：http://gwh.wangdashe.top

[S17] C：安全拼接字符串
来源：http://rrq.hnqzz.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://npn.chenlongwang.top

[S18] C：命令行参数
来源：http://avh.316326.xyz

int main(int argc, char **argv)
来源：http://yel.zycfv.cn

[S19] C：快速排序
来源：http://tqu.yanxiufei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://feg.ydjk.org.cn

[S20] C：二分查找
来源：http://nmb.sxryk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eei.yj20258888.top

[S21] C：字符类别判断
来源：http://nlt.yuxming.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jac.9152youxi.cn

[S22] C：字符串转数字
来源：http://pyo.yvedp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://psf.bbcook.cn

[S23] C：随机数
来源：http://aqn.daria6918.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ydj.zdqjudy.top

[S24] C：获取本地时间
来源：http://bdo.cheryme.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jfm.zycfv.cn

[S25] C：内存拷贝
来源：http://zji.fktsv.cn

memcpy(dst, src, n);
来源：http://nvv.pengpengdd.cyou

[S26] C：内存清零
来源：http://yqv.chenjidiqi.icu

memset(a, 0, sizeof a);
来源：http://tjl.yongpay.top

[S27] C：定义常量
来源：http://mio.jiagoushi.top

const double PI = 3.14159;
来源：http://ahd.zhijiandao.cn

[S28] C：静态变量
来源：http://ftm.ctjpmb.com

static int counter = 0;
来源：http://geg.jinqigufen.top

[S29] C：变参函数
来源：http://eew.sufxvd.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://emg.jinyuanbaomall.cn

[S30] C：头文件保护
来源：http://dln.feifeiyinyue.top

#ifndef X_H
来源：http://aga.zhaomingkeji.xyz

#define X_H
来源：http://fiv.xuanzx.com

#endif
来源：http://kip.yuanzhike.top

[S31] C++：Hello World
来源：http://qag.nanxuanxn.top

#include <iostream>
来源：http://esb.hnqzz.top

int main() { std::cout << "Hello\n"; }
来源：http://gxj.andypj.xyz

[S32] C++：字符串
来源：http://wks.ctjpmb.com

std::string s = "hi";  s += "!";
来源：http://elh.vehdjk.com

[S33] C++：vector 增删
来源：http://tht.c1oappe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://koy.ybcxt.top

[S34] C++：遍历 vector
来源：http://plv.zhaomingkeji.xyz

for (auto &x : v) { std::cout << x; }
来源：http://xki.feifeiyinyue.top

[S35] C++：map
来源：http://opq.zycfv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://iso.svipenyu.cn

[S36] C++：unordered_map
来源：http://dom.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ymg.9152youxi.cn

[S37] C++：set
来源：http://rdj.smart0.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ydp.jinghuilouyu.cn

[S38] C++：排序
来源：http://his.shangyingyoupin.top

std::sort(v.begin(), v.end());
来源：http://fgr.tianlin.xyz

[S39] C++：自定义比较器排序
来源：http://sjj.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fpt.ybcxt.top

[S40] C++：查找元素
来源：http://phn.guannengcc.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://enl.fehbvm.com

[S41] C++：类与构造函数
来源：http://baa.0kj1m.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gpa.chenjidiqi.icu

[S42] C++：继承与虚函数
来源：http://nlh.jyoumei.cn

class B : public Base { public: void f() override {} };
来源：http://tug.xziqi.cn

[S43] C++：智能指针
来源：http://znr.zhaomingkeji.xyz

auto p = std::make_unique<int>(5);
来源：http://und.nanxuanxn.top

[S44] C++：引用传参
来源：http://mze.jqgufenzy.top

void inc(int &x) { ++x; }
来源：http://aiz.iojbl.cn

[S45] C++：lambda
来源：http://cda.ydzc1.top

auto add = [](int a, int b) { return a + b; };
来源：http://wny.sysykeji.top

[S46] C++：函数模板
来源：http://qkw.jinqigfzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bwh.xziqi.cn

[S47] C++：结构化绑定遍历
来源：http://uty.xinyue.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nwz.zhongyouzk.top

[S48] C++：逐行读文件
来源：http://fzf.meibo888.top

std::ifstream in("a.txt");  std::string line;
来源：http://bxl.zhoulong.xyz

while (std::getline(in, line)) { }
来源：http://jsg.yangfankeji.com

[S49] C++：写文件
来源：http://lrs.chenlongwang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://paq.ppjwa.cn

[S50] C++：格式化数字
来源：http://gwd.bbcook.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nsl.zdbjq.cn

[S51] C++：显式类型转换
来源：http://onm.chenjidiqi.icu

static_cast<double>(a) / b
来源：http://dyv.zhijiandao.cn

[S52] C++：const 与 noexcept
来源：http://fsv.ydzc1.top

int size() const noexcept { return n_; }
来源：http://iyp.hammf.cn

[S53] C++：移动语义
来源：http://wbr.ybcxt.top

std::vector<int> w = std::move(v);
来源：http://mrm.hesvh.cn

[S54] C++：异常处理
来源：http://axe.fengsongda.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mhq.svipenyu.cn

[S55] C++：结构化绑定
来源：http://zni.ctjpmb.com

auto [a, b] = std::make_pair(1, 2);
来源：http://ozi.guannengcc.top

[S56] C++：optional
来源：http://xwu.ehwqpu.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://anl.fengsongda.top

[S57] C++：编译期常量
来源：http://jjx.zhijiandao.cn

constexpr int N = 10;
来源：http://wbw.shanyushiyangtech.top

[S58] C++：命名空间
来源：http://dcq.hysaishi.cn

namespace ns { int f() { return 1; } }
来源：http://oys.xingfuxueyuan.xyz

[S59] C++：静态断言
来源：http://nud.shuidangran.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zfv.guannengcc.top

[S60] C++：遍历并删除元素
来源：http://bdv.jinghuilouyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ntv.sufxvd.cn

================================================================================
来源：http://yow.redwolf501.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tke.yuanzhike.top

================================================================================
来源：http://inj.chenlongwang.top

[T01] Kotlin：Hello World
来源：http://rnz.shuidangran.top

println("Hello")
来源：http://ixj.mhx1999.top

[T02] Kotlin：变量
来源：http://znd.ydzc1.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cbo.jqgufenzy.top

[T03] Kotlin：字符串模板
来源：http://phg.yj20258888.top

"值: $b"
来源：http://zzf.zhixingplan.top

[T04] Kotlin：空安全
来源：http://wdj.jqgufenzy.top

val n: String? = null;  n?.length
来源：http://czw.tianlin.xyz

[T05] Kotlin：when 表达式
来源：http://exz.jlsjyb.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mex.yangfankeji.com

[T06] Kotlin：集合映射
来源：http://wuk.jiagoushi.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ofm.shuidangran.top


<!-- 参考信息 -->