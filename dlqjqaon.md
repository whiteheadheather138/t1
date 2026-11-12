代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bsy.ehwqpu.com

[R08] 数值比较
来源：http://ofu.hywenlv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://peh.0kj1m.cn

[R09] 字符串比较
来源：http://mtz.yj20258888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wqd.daria6918.cn

[R10] 正则匹配
来源：http://irv.52xcode.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://smc.hnqzz.top

[R11] case 多分支
来源：http://euu.hywenlv.cn

case "$1" in
来源：http://fll.sjlbkw.cn

start) echo "启动" ;;
来源：http://zzq.gotoacloud.top

stop)  echo "停止" ;;
来源：http://lvr.zdbjq.cn

*)     echo "未知命令" ;;
来源：http://lio.hnqzz.top

esac
来源：http://ydp.ctjpmb.com

[R12] for 遍历文件
来源：http://wke.chenzaomai.com

for f in *.txt; do echo "$f"; done
来源：http://adv.wangshuangyany.cn

[R13] for 计数循环
来源：http://dfi.jinqigufen.top

for i in {1..10}; do echo "$i"; done
来源：http://kiy.birdmap.top

[R14] C 风格 for
来源：http://hyo.jiagoushi.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uyh.gogol.net.cn

[R15] while 逐行读文件
来源：http://wyq.chenlongwang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ldf.fktsv.cn

[R16] until 等待条件
来源：http://hmd.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wsx.jqgufenzy.top

[R17] 数组定义与取值
来源：http://zys.cucudq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kot.cheryme.top

[R18] 遍历数组
来源：http://emv.nwbrower.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rdj.hnqzz.top

[R19] 数组长度
来源：http://fcf.ctjpmb.com

echo "${#arr[@]}"
来源：http://iis.vehdjk.com

[R20] 关联数组（字典）
来源：http://aiq.hongshengwenyu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mvk.wangshuangyany.cn

[R21] 字符串长度
来源：http://yqn.andypj.xyz

echo "${#s}"
来源：http://dcg.jyoumei.cn

[R22] 截取子串
来源：http://ifp.fktsv.cn

echo "${s:0:5}"
来源：http://pfl.fzhhl.top

[R23] 字符串替换
来源：http://btc.vqdsnc.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pct.aibaodan.cn

[R24] 大小写转换
来源：http://mur.cdnleiting.top

echo "${s^^}"; echo "${s,,}"
来源：http://mpb.wangdashe.top

[R25] 去后缀 / 去前缀
来源：http://oev.jiagoushi.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ame.iojbl.cn

[R26] 命令替换
来源：http://ebx.birdmap.top

now=$(date +%F); echo "$now"
来源：http://bad.316326.xyz

[R27] 算术展开
来源：http://wvk.yj20258888.top

echo $((1 + 2 * 3))
来源：http://oun.nanxuanxn.top

[R28] 浮点运算
来源：http://gna.sxryk.cn

echo "scale=2; 10/3" | bc
来源：http://toe.zhixingplan.top

[R29] 定义函数
来源：http://bke.sjlbkw.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blv.bjfxy.top

[R30] 函数返回状态码
来源：http://jfm.zhaomingkeji.xyz

f() { return 0; }; f || echo "失败了"
来源：http://dhj.nanxinkj.top

[R31] 局部变量
来源：http://qsy.shzxlz.cn

f() { local x=1; echo "$x"; }
来源：http://unx.shangyingyoupin.top

[R32] 参数个数校验
来源：http://uup.xinyue.icu

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://erf.fanxiaobao.xyz

[R33] 捕获错误并提示行号
来源：http://jcl.haohaochexian.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://znb.uphjek.com

[R34] 退出时清理
来源：http://pum.bbcook.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ckj.snrcjt.cn

[R35] 后台执行并等待
来源：http://gyv.9152youxi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xsd.hongshengwenyu.top

[R36] 并发执行多个任务
来源：http://dmp.jianghu66.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mmv.xingfuxueyuan.xyz

[R37] 把输出赋给变量
来源：http://bmv.mhx1999.top

files=$(ls -1)
来源：http://zth.ydjk.org.cn

[R38] 管道串联
来源：http://phc.chenlongwang.top

cat a.txt | grep -i error | wc -l
来源：http://qnc.gzhubu.top

[R39] 重定向标准输出与错误
来源：http://klu.nanxinkj.top

cmd > out.log 2>&1
来源：http://ayw.zdqjudy.top

[R40] 追加写日志
来源：http://yvd.vqdsnc.cn

echo "log" >> out.log
来源：http://rcc.tarul.cn

[R41] 丢弃输出
来源：http://xui.hammf.cn

cmd >/dev/null 2>&1
来源：http://uql.snrcjt.cn

[R42] 输入重定向
来源：http://bke.shzxlz.cn

wc -l < a.txt
来源：http://zgk.52xcode.cn

[R43] 按名字查找文件
来源：http://bjp.zhiwuduotai.top

find . -name "*.log" -type f
来源：http://qpj.jqgfzy.top

[R44] 按修改时间查找
来源：http://zpp.zdbjq.cn

find . -mtime -7 -type f
来源：http://mzz.cashguo.top

[R45] 批量删除
来源：http://bsn.nanxinkj.top

find . -name "*.tmp" -delete
来源：http://fnw.yj20258888.top

[R46] 递归替换文件内容
来源：http://dvx.xingfuxueyuan.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pzl.shangyingyoupin.top

[R47] sed 单行替换
来源：http://iqe.vqdsnc.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vxl.svipenyu.cn

[R48] awk 取指定列
来源：http://pwt.meibo888.top

awk '{print $1, $3}' a.txt
来源：http://yee.ybcxt.top

[R49] awk 带条件
来源：http://vza.jinqigufen.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dwe.gzhubu.top

[R50] awk 求和
来源：http://baq.ehwqpu.com

awk '{s += $2} END {print s}' a.txt
来源：http://vec.gaohongyu789.top

[R51] 排序去重取前几
来源：http://aye.nanxinkj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://wyi.hnxiangtu.top

[R52] 统计行数
来源：http://klm.dashuyun.cn

wc -l a.txt
来源：http://tek.yfazqb.com

[R53] 查看文件头与实时尾
来源：http://kjx.jyoumei.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ipv.jinqigfzy.top

[R54] 比较两个文件
来源：http://zqe.aibaodan.cn

diff a.txt b.txt
来源：http://olt.yueranfly.top

[R55] 压缩与解压
来源：http://lcv.svipenyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hmh.tianlin.xyz

[R56] 远程拷贝
来源：http://izl.chenjidiqi.icu

scp file user@host:/path/
来源：http://rtv.tarul.cn

[R57] 远程执行命令
来源：http://btv.yj20258888.top

ssh user@host 'uptime'
来源：http://cpt.tian-w.cn

[R58] 下载文件
来源：http://xdf.smart0.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fqw.ehwqpu.com

[R59] 发 POST JSON
来源：http://vmq.shanyushiyangtech.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nho.yfazqb.com

[R60] 只看 HTTP 状态码
来源：http://dob.zhongyouzk.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kme.cqqwz.cn

[R61] 磁盘占用
来源：http://htp.fengsongda.top

df -h;  du -sh *
来源：http://ijl.xziqi.cn

[R62] 找最占空间的文件
来源：http://wcz.cdnleiting.top

du -ah . | sort -rh | head -10
来源：http://kfa.smart0.xyz

[R63] 内存与进程
来源：http://erg.andypj.xyz

free -h;  ps aux | grep nginx
来源：http://xuf.yfazqb.com

[R64] 结束进程
来源：http://hai.sjlbkw.cn

kill -9 $(pgrep -f app.py)
来源：http://rwo.xingfuxueyuan.xyz

[R65] 查看端口占用
来源：http://tod.yj202588.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://krf.bjfxy.top

[R66] 定时任务
来源：http://kdp.52xcode.cn

crontab -e;  crontab -l
来源：http://vty.jinqigfzy.top

[R67] 生成随机十六进制串
来源：http://mll.svipenyu.cn

openssl rand -hex 16
来源：http://qro.vehdjk.com

[R68] 计算文件校验值
来源：http://ezh.gzhubu.top

sha256sum a.txt;  md5sum a.txt
来源：http://icq.uphjek.com

[R69] 生成随机密码
来源：http://jxe.sufxvd.cn

head -c 16 /dev/urandom | base64
来源：http://aur.epnwcf.com

[R70] 时间戳与互转
来源：http://qxu.sjlbkw.cn

date +%s;  date -d @1700000000
来源：http://jby.mhx1999.top

[R71] 日期格式化
来源：http://dnf.shzxlz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ryd.ehwqpu.com

[R72] 等待端口就绪
来源：http://gzh.epnwcf.com

until nc -z localhost 3306; do sleep 1; done
来源：http://sfa.cheryme.top

[R73] 分割大日志
来源：http://bti.yvedp.cn

split -l 1000 big.log part_
来源：http://vyt.xinyue.icu

[R74] 批量重命名
来源：http://bot.yvedp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gee.yanxiufei.cn

[R75] 导出环境变量
来源：http://pno.yj202588.top

export PATH="$HOME/bin:$PATH"
来源：http://haw.gaohongyu789.top

[R76] 使用临时文件
来源：http://uom.0kj1m.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dib.zhengqikj.top

[R77] 读取用户输入
来源：http://tjc.jyoumei.cn

read -rp "请输入: " ans
来源：http://ttn.zycfv.cn

[R78] 交互式菜单
来源：http://tfw.snrcjt.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://eyo.epnwcf.com

[R79] 解析命令行选项
来源：http://hlx.ywan-chungtsiang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gfe.yongpay.top

[R80] 查看脚本执行耗时
来源：http://dym.9152youxi.cn

time ./run.sh
来源：http://aob.smart0.xyz

================================================================================
来源：http://lzl.tian-w.cn

S. C / C++ 专题
来源：http://wxb.iojbl.cn

================================================================================
来源：http://hxl.ctjpmb.com

[S01] C：Hello World
来源：http://ved.zhiwuduotai.top

#include <stdio.h>
来源：http://sai.tian-w.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qef.snrcjt.cn

[S02] C：变量与格式化输出
来源：http://xlz.xingfuxueyuan.xyz

int a = 10; printf("%d\n", a);
来源：http://yme.zdqjudy.top

[S03] C：读入整数
来源：http://jxv.guannengcc.top

int x; scanf("%d", &x);
来源：http://bfm.9152youxi.cn

[S04] C：字符串复制
来源：http://hjy.fanxiaobao.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://czu.52xcode.cn

[S05] C：字符串长度
来源：http://sgj.jiagoushi.top

strlen(s)
来源：http://xpc.zhengqikj.top

[S06] C：字符串比较
来源：http://moe.vehdjk.com

strcmp(a, b) == 0
来源：http://lny.birdmap.top

[S07] C：数组遍历求和
来源：http://gzm.cucudq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cys.hnqzz.top

[S08] C：动态内存分配与释放
来源：http://sjg.nanxinkj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jhj.hfpthk.cn

[S09] C：结构体定义与初始化
来源：http://mls.hammf.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://afp.hesvh.cn

[S10] C：指针与解引用
来源：http://ucz.pycfn.com

int *p = &a;  *p = 5;
来源：http://qud.jlsjyb.cn

[S11] C：逐行读文件
来源：http://ljs.ydjk.org.cn

FILE *f = fopen("a.txt", "r");
来源：http://mqp.daria6918.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ngk.xylfe.cn

fclose(f);
来源：http://hof.zhaomingkeji.xyz

[S12] C：写文件
来源：http://rau.hywenlv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tbg.xylfe.cn

[S13] C：宏定义
来源：http://dcx.ybcxt.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bxv.svipenyu.cn

[S14] C：枚举
来源：http://mms.xylfe.cn

enum Color { RED, GREEN, BLUE };
来源：http://uhh.bjfxy.top

[S15] C：类型转换
来源：http://kpz.gaohongyu789.top

(double) a / b
来源：http://mfm.yonumen.top

[S16] C：位操作置位
来源：http://bev.fanxiaobao.xyz

x |= (1 << 3);
来源：http://oab.fktsv.cn

[S17] C：安全拼接字符串
来源：http://vlk.hysaishi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://npk.wangdashe.top

[S18] C：命令行参数
来源：http://ufm.c1oappe.top

int main(int argc, char **argv)
来源：http://wia.jinghuilouyu.cn

[S19] C：快速排序
来源：http://okb.smart0.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://tlw.yuxming.cn

[S20] C：二分查找
来源：http://kfa.jiagoushi.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://glq.shangyingyoupin.top

[S21] C：字符类别判断
来源：http://lxj.guannengcc.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xkr.fengsongda.top

[S22] C：字符串转数字
来源：http://xhd.jinyuanbaomall.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bho.jinqigufen.top

[S23] C：随机数
来源：http://ruq.mhx1999.top

srand(time(NULL));  int r = rand() % 100;
来源：http://sjt.zhaomingkeji.xyz

[S24] C：获取本地时间
来源：http://mhl.redwolf501.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jbn.yonumen.top

[S25] C：内存拷贝
来源：http://wjv.xuanzx.com

memcpy(dst, src, n);
来源：http://kkj.xuetiantiany.cn

[S26] C：内存清零
来源：http://tfl.ywan-chungtsiang.top

memset(a, 0, sizeof a);
来源：http://yns.yj20258888.top

[S27] C：定义常量
来源：http://vjl.jinqigufen.top

const double PI = 3.14159;
来源：http://jrd.hcnkem.com

[S28] C：静态变量
来源：http://rts.tanke756.top

static int counter = 0;
来源：http://evh.zdbjq.cn

[S29] C：变参函数
来源：http://ugz.daxiang520.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pzb.ydjk.org.cn

[S30] C：头文件保护
来源：http://dyh.hesvh.cn

#ifndef X_H
来源：http://byp.pengpengdd.cyou

#define X_H
来源：http://gsl.zhongyouzk.top

#endif
来源：http://omy.yueranfly.top

[S31] C++：Hello World
来源：http://wsc.ppjwa.cn

#include <iostream>
来源：http://mva.nwbrower.top

int main() { std::cout << "Hello\n"; }
来源：http://opm.zycfv.cn

[S32] C++：字符串
来源：http://let.hcnkem.com

std::string s = "hi";  s += "!";
来源：http://vhl.fanxiaobao.xyz

[S33] C++：vector 增删
来源：http://fco.wangshuangyany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dfk.gaohongyu789.top

[S34] C++：遍历 vector
来源：http://xko.shangyingyoupin.top

for (auto &x : v) { std::cout << x; }
来源：http://knb.haohaochexian.top

[S35] C++：map
来源：http://dtw.hysaishi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qxp.daria6918.cn

[S36] C++：unordered_map
来源：http://qam.nanxinkj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ujz.feifeiyinyue.top

[S37] C++：set
来源：http://alt.yj20258.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fim.tanke756.top

[S38] C++：排序
来源：http://zbo.jinyuanbaomall.cn

std::sort(v.begin(), v.end());
来源：http://fvl.jinqigfzy.top

[S39] C++：自定义比较器排序
来源：http://tbj.zhongyouzk.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zco.sjlbkw.cn

[S40] C++：查找元素
来源：http://oim.nanxinkj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zeb.yuanzhike.top

[S41] C++：类与构造函数
来源：http://lof.ydzc1.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mwv.cqqwz.cn

[S42] C++：继承与虚函数
来源：http://qwq.havefunace.top

class B : public Base { public: void f() override {} };
来源：http://vkm.hysaishi.cn

[S43] C++：智能指针
来源：http://tjq.zycfv.cn

auto p = std::make_unique<int>(5);
来源：http://cud.wangdashe.top

[S44] C++：引用传参
来源：http://igj.quarkkingdee.top

void inc(int &x) { ++x; }
来源：http://knb.hongshengwenyu.top

[S45] C++：lambda
来源：http://kii.sysykeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://krx.pycfn.com

[S46] C++：函数模板
来源：http://oqe.uphjek.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://urp.pycfn.com

[S47] C++：结构化绑定遍历
来源：http://vch.yuanzhike.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fvp.epnwcf.com

[S48] C++：逐行读文件
来源：http://lzl.hcnkem.com

std::ifstream in("a.txt");  std::string line;
来源：http://ssc.tianlin.xyz

while (std::getline(in, line)) { }
来源：http://ftq.9152youxi.cn

[S49] C++：写文件
来源：http://hsb.birdmap.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yoz.ppjwa.cn

[S50] C++：格式化数字
来源：http://dxh.xuanzx.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hbf.zycfv.cn

[S51] C++：显式类型转换
来源：http://bdr.jiagoushi.top

static_cast<double>(a) / b
来源：http://pmr.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://xbh.ppjwa.cn

int size() const noexcept { return n_; }
来源：http://xsp.tanke756.top

[S53] C++：移动语义
来源：http://okf.zhoulong.xyz

std::vector<int> w = std::move(v);
来源：http://imc.quarkkingdee.top

[S54] C++：异常处理
来源：http://zch.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gft.ydzc1.top

[S55] C++：结构化绑定
来源：http://ila.gzhubu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ryk.smart0.xyz

[S56] C++：optional
来源：http://sky.cheryme.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yjm.tianlin.xyz

[S57] C++：编译期常量
来源：http://ugk.hammf.cn

constexpr int N = 10;
来源：http://imt.zhongyouzk.top

[S58] C++：命名空间
来源：http://omi.ctjpmb.com

namespace ns { int f() { return 1; } }
来源：http://wum.jlsjyb.cn

[S59] C++：静态断言
来源：http://vsm.wangshuangyany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tps.hesvh.cn

[S60] C++：遍历并删除元素
来源：http://btg.jinyuanbaomall.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qpr.guannengcc.top

================================================================================
来源：http://ilq.havefunace.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lud.ydzc1.top

================================================================================
来源：http://utz.chenlongwang.top

[T01] Kotlin：Hello World
来源：http://wqm.zhiwuduotai.top

println("Hello")
来源：http://jzo.ivvv.top

[T02] Kotlin：变量
来源：http://tjx.hongshengwenyu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lny.shuidangran.top

[T03] Kotlin：字符串模板
来源：http://cqx.9152youxi.cn

"值: $b"
来源：http://und.jinqigfzy.top

[T04] Kotlin：空安全
来源：http://ese.guannengcc.top

val n: String? = null;  n?.length
来源：http://wwi.hnxiangtu.top

[T05] Kotlin：when 表达式
来源：http://ola.chenlongwang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lmn.yangfankeji.com

[T06] Kotlin：集合映射
来源：http://xmn.yongpay.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hhn.fanxiaobao.xyz

[T07] Kotlin：集合过滤
来源：http://opg.yfazqb.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://bnz.daxiang520.top

[T08] Kotlin：数据类
来源：http://xmr.aibaodan.cn

data class User(val name: String, val age: Int)
来源：http://rtl.ybcxt.top


<!-- 参考信息 -->