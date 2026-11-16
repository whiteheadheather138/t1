代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zbf.hcnkem.com

[R10] 正则匹配
来源：http://zyn.ehwqpu.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vpr.jiagoushi.top

[R11] case 多分支
来源：http://igt.hongshengwenyu.top

case "$1" in
来源：http://iye.sufxvd.cn

start) echo "启动" ;;
来源：http://zfd.sxryk.cn

stop)  echo "停止" ;;
来源：http://zye.fengsongda.top

*)     echo "未知命令" ;;
来源：http://kko.ydzc1.top

esac
来源：http://dlk.gaohongyu789.top

[R12] for 遍历文件
来源：http://xau.yj202588.top

for f in *.txt; do echo "$f"; done
来源：http://qib.jinqigfzy.top

[R13] for 计数循环
来源：http://bra.redwolf501.top

for i in {1..10}; do echo "$i"; done
来源：http://qia.ybcxt.top

[R14] C 风格 for
来源：http://odb.uphjek.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://faa.quarkkingdee.top

[R15] while 逐行读文件
来源：http://rom.cucudq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yic.hnxiangtu.top

[R16] until 等待条件
来源：http://vbk.shanyushiyangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nzh.sysykeji.top

[R17] 数组定义与取值
来源：http://tut.nwbrower.top

arr=(a b c); echo "${arr[0]}"
来源：http://keb.jqgufenzy.top

[R18] 遍历数组
来源：http://vug.sweek.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lly.jqgufenzy.top

[R19] 数组长度
来源：http://iuy.c1oappe.top

echo "${#arr[@]}"
来源：http://fcv.zycfv.cn

[R20] 关联数组（字典）
来源：http://tua.guowangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://czg.hcnkem.com

[R21] 字符串长度
来源：http://fxj.meibo888.top

echo "${#s}"
来源：http://tmj.nanxinkj.top

[R22] 截取子串
来源：http://ocn.ydzc1.top

echo "${s:0:5}"
来源：http://gqm.yongpay.top

[R23] 字符串替换
来源：http://yzc.chenjidiqi.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://drt.birdmap.top

[R24] 大小写转换
来源：http://wnu.gotoacloud.top

echo "${s^^}"; echo "${s,,}"
来源：http://sev.epnwcf.com

[R25] 去后缀 / 去前缀
来源：http://ekm.xingfuxueyuan.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://ruj.jiagoushi.top

[R26] 命令替换
来源：http://gwg.snrcjt.cn

now=$(date +%F); echo "$now"
来源：http://aze.birdmap.top

[R27] 算术展开
来源：http://nhp.shuidangran.top

echo $((1 + 2 * 3))
来源：http://std.guowangkeji.top

[R28] 浮点运算
来源：http://vtb.zhaomingkeji.xyz

echo "scale=2; 10/3" | bc
来源：http://rtj.zhixingplan.top

[R29] 定义函数
来源：http://dov.yanxiufei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gto.yongpay.top

[R30] 函数返回状态码
来源：http://jsa.gogol.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://vbo.xuetiantiany.cn

[R31] 局部变量
来源：http://rci.hnqzz.top

f() { local x=1; echo "$x"; }
来源：http://nrf.yanxiufei.cn

[R32] 参数个数校验
来源：http://jib.xziqi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ykv.yueranfly.top

[R33] 捕获错误并提示行号
来源：http://ywo.chenzaomai.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nof.chenjidiqi.icu

[R34] 退出时清理
来源：http://ikk.jyoumei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nfy.jinyuanbaomall.cn

[R35] 后台执行并等待
来源：http://raz.52xcode.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xuu.jlsjyb.cn

[R36] 并发执行多个任务
来源：http://wre.gaohongyu789.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rsf.jinyuanbaomall.cn

[R37] 把输出赋给变量
来源：http://ouw.smart0.xyz

files=$(ls -1)
来源：http://oig.chenzaomai.com

[R38] 管道串联
来源：http://frz.tarul.cn

cat a.txt | grep -i error | wc -l
来源：http://xib.cheryme.top

[R39] 重定向标准输出与错误
来源：http://eye.fengsongda.top

cmd > out.log 2>&1
来源：http://ibm.jianghu66.top

[R40] 追加写日志
来源：http://qsa.hnqzz.top

echo "log" >> out.log
来源：http://nvr.jlsjyb.cn

[R41] 丢弃输出
来源：http://gps.havefunace.top

cmd >/dev/null 2>&1
来源：http://aay.havefunace.top

[R42] 输入重定向
来源：http://bpm.jlsjyb.cn

wc -l < a.txt
来源：http://scu.havefunace.top

[R43] 按名字查找文件
来源：http://vny.hcnkem.com

find . -name "*.log" -type f
来源：http://dhj.yj20258888.top

[R44] 按修改时间查找
来源：http://mwy.redwolf501.top

find . -mtime -7 -type f
来源：http://ive.hfpthk.cn

[R45] 批量删除
来源：http://ona.yonumen.top

find . -name "*.tmp" -delete
来源：http://ngx.ydjk.org.cn

[R46] 递归替换文件内容
来源：http://znn.yuxming.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yhb.yuxming.cn

[R47] sed 单行替换
来源：http://doq.yj20258888.top

sed -i 's/foo/bar/g' a.txt
来源：http://blf.fengsongda.top

[R48] awk 取指定列
来源：http://fjs.jinqigfzy.top

awk '{print $1, $3}' a.txt
来源：http://mqf.sweek.top

[R49] awk 带条件
来源：http://epg.xylfe.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pwg.0kj1m.cn

[R50] awk 求和
来源：http://ait.sysykeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://zhd.zhixingplan.top

[R51] 排序去重取前几
来源：http://sxv.zhoulong.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://mcm.cucudq.cn

[R52] 统计行数
来源：http://izq.yuanzhike.top

wc -l a.txt
来源：http://itb.jqgfzy.top

[R53] 查看文件头与实时尾
来源：http://qrt.yfazqb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://plt.fzhhl.top

[R54] 比较两个文件
来源：http://bot.svipenyu.cn

diff a.txt b.txt
来源：http://dqw.jiagoushi.top

[R55] 压缩与解压
来源：http://fqf.guowangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://arm.yvedp.cn

[R56] 远程拷贝
来源：http://fbk.cdnleiting.top

scp file user@host:/path/
来源：http://csa.xziqi.cn

[R57] 远程执行命令
来源：http://zjc.yvedp.cn

ssh user@host 'uptime'
来源：http://llz.jyoumei.cn

[R58] 下载文件
来源：http://vks.yanxiufei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zgn.redwolf501.top

[R59] 发 POST JSON
来源：http://vau.ctjpmb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kcw.sysykeji.top

[R60] 只看 HTTP 状态码
来源：http://ajg.yj20258888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wix.zhixingplan.top

[R61] 磁盘占用
来源：http://xtr.nwbrower.top

df -h;  du -sh *
来源：http://lnm.hnqzz.top

[R62] 找最占空间的文件
来源：http://gvn.xziqi.cn

du -ah . | sort -rh | head -10
来源：http://ncq.ywan-chungtsiang.top

[R63] 内存与进程
来源：http://srz.ctjpmb.com

free -h;  ps aux | grep nginx
来源：http://onf.dashuyun.cn

[R64] 结束进程
来源：http://ame.jqgufenzy.top

kill -9 $(pgrep -f app.py)
来源：http://vum.cheryme.top

[R65] 查看端口占用
来源：http://ryv.gaohongyu789.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wfl.zycfv.cn

[R66] 定时任务
来源：http://gcz.epnwcf.com

crontab -e;  crontab -l
来源：http://lqv.cdnleiting.top

[R67] 生成随机十六进制串
来源：http://gtz.xziqi.cn

openssl rand -hex 16
来源：http://gza.daria6918.cn

[R68] 计算文件校验值
来源：http://dhq.ppjwa.cn

sha256sum a.txt;  md5sum a.txt
来源：http://aag.dashuyun.cn

[R69] 生成随机密码
来源：http://quh.guowangkeji.top

head -c 16 /dev/urandom | base64
来源：http://yhx.fktsv.cn

[R70] 时间戳与互转
来源：http://rvf.chenjidiqi.icu

date +%s;  date -d @1700000000
来源：http://bhx.zhongyouzk.top

[R71] 日期格式化
来源：http://mtp.zdbjq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hkn.jianghu66.top

[R72] 等待端口就绪
来源：http://ktt.chenlongwang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hwi.tarul.cn

[R73] 分割大日志
来源：http://vfh.xziqi.cn

split -l 1000 big.log part_
来源：http://bmf.yuanzhike.top

[R74] 批量重命名
来源：http://see.pycfn.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cpb.shanyushiyangkeji.top

[R75] 导出环境变量
来源：http://yzc.xuetiantiany.cn

export PATH="$HOME/bin:$PATH"
来源：http://yoj.zdbjq.cn

[R76] 使用临时文件
来源：http://tkl.hesvh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nya.yj20258.top

[R77] 读取用户输入
来源：http://qnz.jianghu66.top

read -rp "请输入: " ans
来源：http://nee.hammf.cn

[R78] 交互式菜单
来源：http://eik.haohaochexian.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ffj.hammf.cn

[R79] 解析命令行选项
来源：http://iej.uphjek.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jhd.sxryk.cn

[R80] 查看脚本执行耗时
来源：http://llr.yangfankeji.com

time ./run.sh
来源：http://dfk.zhixingplan.top

================================================================================
来源：http://wil.bbcook.cn

S. C / C++ 专题
来源：http://erg.xziqi.cn

================================================================================
来源：http://zgj.jianghu66.top

[S01] C：Hello World
来源：http://lln.jqgufenzy.top

#include <stdio.h>
来源：http://ahx.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qog.hnqzz.top

[S02] C：变量与格式化输出
来源：http://qow.ivvv.top

int a = 10; printf("%d\n", a);
来源：http://sak.zhongyouzk.top

[S03] C：读入整数
来源：http://the.yuanzhike.top

int x; scanf("%d", &x);
来源：http://ixr.ctjpmb.com

[S04] C：字符串复制
来源：http://rsy.xingfuxueyuan.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://ejh.tanke756.top

[S05] C：字符串长度
来源：http://kwf.smart0.xyz

strlen(s)
来源：http://rzo.0kj1m.cn

[S06] C：字符串比较
来源：http://sva.shzxlz.cn

strcmp(a, b) == 0
来源：http://cml.snrcjt.cn

[S07] C：数组遍历求和
来源：http://ups.hysaishi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yau.fktsv.cn

[S08] C：动态内存分配与释放
来源：http://cwg.gotoacloud.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ofs.yfazqb.com

[S09] C：结构体定义与初始化
来源：http://vpo.fzhhl.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ckn.andypj.xyz

[S10] C：指针与解引用
来源：http://njz.chenjidiqi.icu

int *p = &a;  *p = 5;
来源：http://zfk.hfpthk.cn

[S11] C：逐行读文件
来源：http://cnd.xingfuxueyuan.xyz

FILE *f = fopen("a.txt", "r");
来源：http://ryp.hnqzz.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://owl.ydzc1.top

fclose(f);
来源：http://czb.hammf.cn

[S12] C：写文件
来源：http://srr.cqqwz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://shd.jinyuanbaomall.cn

[S13] C：宏定义
来源：http://qpe.guowangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xxg.hesvh.cn

[S14] C：枚举
来源：http://slc.zhiwuduotai.top

enum Color { RED, GREEN, BLUE };
来源：http://vhq.hysaishi.cn

[S15] C：类型转换
来源：http://ych.feifeiyinyue.top

(double) a / b
来源：http://bwc.ivvv.top

[S16] C：位操作置位
来源：http://mty.zhoulong.xyz

x |= (1 << 3);
来源：http://nbx.hnqzz.top

[S17] C：安全拼接字符串
来源：http://vpz.hesvh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gnw.chenjidiqi.icu

[S18] C：命令行参数
来源：http://zat.jinqigfzy.top

int main(int argc, char **argv)
来源：http://hhb.quarkkingdee.top

[S19] C：快速排序
来源：http://ste.jqgfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://jgz.tanke756.top

[S20] C：二分查找
来源：http://awy.hammf.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://udb.tanke756.top

[S21] C：字符类别判断
来源：http://tuj.zdqjudy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://scd.cashguo.top

[S22] C：字符串转数字
来源：http://zre.hammf.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uas.nwbrower.top

[S23] C：随机数
来源：http://lnv.0kj1m.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://imy.bbcook.cn

[S24] C：获取本地时间
来源：http://jdq.ywan-chungtsiang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ehb.zhoulong.xyz

[S25] C：内存拷贝
来源：http://rid.xziqi.cn

memcpy(dst, src, n);
来源：http://nfn.ywan-chungtsiang.top

[S26] C：内存清零
来源：http://jya.xingfuxueyuan.xyz

memset(a, 0, sizeof a);
来源：http://chq.fengsongda.top

[S27] C：定义常量
来源：http://cwr.zhiwuduotai.top

const double PI = 3.14159;
来源：http://fol.jinghuilouyu.cn

[S28] C：静态变量
来源：http://awl.sysykeji.top

static int counter = 0;
来源：http://jem.pycfn.com

[S29] C：变参函数
来源：http://nkw.zycfv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jio.yj20258888.top

[S30] C：头文件保护
来源：http://uzz.gotoacloud.top

#ifndef X_H
来源：http://twl.guowangkeji.top

#define X_H
来源：http://mng.aizwys.cn

#endif
来源：http://srj.52xcode.cn

[S31] C++：Hello World
来源：http://gxs.meibo888.top

#include <iostream>
来源：http://pnl.bjfxy.top

int main() { std::cout << "Hello\n"; }
来源：http://kmk.yuxming.cn

[S32] C++：字符串
来源：http://hre.fehbvm.com

std::string s = "hi";  s += "!";
来源：http://ziu.zhoulong.xyz

[S33] C++：vector 增删
来源：http://rbj.jinghuilouyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yzv.gzhubu.top

[S34] C++：遍历 vector
来源：http://qnr.yfazqb.com

for (auto &x : v) { std::cout << x; }
来源：http://imk.ydzc1.top

[S35] C++：map
来源：http://hbk.shangyingyoupin.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cnt.daria6918.cn

[S36] C++：unordered_map
来源：http://djf.cashguo.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kcu.guannengcc.top

[S37] C++：set
来源：http://yjv.ctjpmb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ghh.aizwys.cn

[S38] C++：排序
来源：http://kyv.52xcode.cn

std::sort(v.begin(), v.end());
来源：http://wbo.yfazqb.com

[S39] C++：自定义比较器排序
来源：http://rkt.jinghuilouyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ccx.zdbjq.cn

[S40] C++：查找元素
来源：http://khf.ehwqpu.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hxt.gaohongyu789.top

[S41] C++：类与构造函数
来源：http://zdx.nanxuanxn.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ucr.cucudq.cn

[S42] C++：继承与虚函数
来源：http://znb.c1oappe.top

class B : public Base { public: void f() override {} };
来源：http://fre.fehbvm.com

[S43] C++：智能指针
来源：http://wcq.hcnkem.com

auto p = std::make_unique<int>(5);
来源：http://syc.fzhhl.top

[S44] C++：引用传参
来源：http://tvc.0kj1m.cn

void inc(int &x) { ++x; }
来源：http://pfu.hammf.cn

[S45] C++：lambda
来源：http://jur.hnxiangtu.top

auto add = [](int a, int b) { return a + b; };
来源：http://pdl.yuanzhike.top

[S46] C++：函数模板
来源：http://pwo.chenjidiqi.icu

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tgg.fanxiaobao.xyz

[S47] C++：结构化绑定遍历
来源：http://epn.fehbvm.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bok.zhijiandao.cn

[S48] C++：逐行读文件
来源：http://mpx.shuidangran.top

std::ifstream in("a.txt");  std::string line;
来源：http://cye.nwbrower.top

while (std::getline(in, line)) { }
来源：http://rro.jqgufenzy.top

[S49] C++：写文件
来源：http://wlk.jianghu66.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ygu.vehdjk.com

[S50] C++：格式化数字
来源：http://odb.gogol.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ppd.zhiwuduotai.top

[S51] C++：显式类型转换
来源：http://gcl.ybcxt.top

static_cast<double>(a) / b
来源：http://ejt.jinyuanbaomall.cn

[S52] C++：const 与 noexcept
来源：http://xaz.haohaochexian.top

int size() const noexcept { return n_; }
来源：http://eut.zhengqikj.top

[S53] C++：移动语义
来源：http://ykk.cucudq.cn

std::vector<int> w = std::move(v);
来源：http://klc.52xcode.cn

[S54] C++：异常处理
来源：http://cgk.gotoacloud.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ltp.nanxinkj.top

[S55] C++：结构化绑定
来源：http://dbe.sysykeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xta.tian-w.cn

[S56] C++：optional
来源：http://hxy.vqdsnc.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://unn.sufxvd.cn

[S57] C++：编译期常量
来源：http://hss.tian-w.cn

constexpr int N = 10;
来源：http://onw.xylfe.cn

[S58] C++：命名空间
来源：http://ize.pycfn.com

namespace ns { int f() { return 1; } }
来源：http://bvy.yueranfly.top

[S59] C++：静态断言
来源：http://erw.fzhhl.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bkp.ivvv.top

[S60] C++：遍历并删除元素
来源：http://gip.yangfankeji.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://edu.jqgfzy.top

================================================================================
来源：http://ocb.guowangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eby.zhengqikj.top

================================================================================
来源：http://vfj.snrcjt.cn

[T01] Kotlin：Hello World
来源：http://eqh.tian-w.cn

println("Hello")
来源：http://mhx.cheryme.top

[T02] Kotlin：变量
来源：http://luw.hongshengwenyu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oec.jlsjyb.cn

[T03] Kotlin：字符串模板
来源：http://pet.yj20258.top

"值: $b"
来源：http://hdu.gogol.net.cn

[T04] Kotlin：空安全
来源：http://pln.shuidangran.top

val n: String? = null;  n?.length
来源：http://eef.wangdashe.top

[T05] Kotlin：when 表达式
来源：http://fdf.nanxuanxn.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tin.ywan-chungtsiang.top

[T06] Kotlin：集合映射
来源：http://osx.xinyue.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://msc.shangyingyoupin.top

[T07] Kotlin：集合过滤
来源：http://zqj.yj20258888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rzr.xinyue.icu

[T08] Kotlin：数据类
来源：http://bea.tianlin.xyz

data class User(val name: String, val age: Int)
来源：http://zxc.zdbjq.cn

[T09] Kotlin：扩展函数
来源：http://dzw.haohaochexian.top

fun String.exclaim() = this + "!"
来源：http://zoq.nwbrower.top

[T10] Kotlin：默认参数
来源：http://vai.tianlin.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://tet.cqqwz.cn


<!-- 参考信息 -->