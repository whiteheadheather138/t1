代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://ywk.meibo888.top

[R18] 遍历数组
来源：http://fat.ydzc1.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iqi.yongpay.top

[R19] 数组长度
来源：http://knz.yvedp.cn

echo "${#arr[@]}"
来源：http://nft.jlsjyb.cn

[R20] 关联数组（字典）
来源：http://bgk.xingfuxueyuan.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vop.tian-w.cn

[R21] 字符串长度
来源：http://fgb.snrcjt.cn

echo "${#s}"
来源：http://dbb.cashguo.top

[R22] 截取子串
来源：http://bvj.dianchejie.cn

echo "${s:0:5}"
来源：http://qlc.xziqi.cn

[R23] 字符串替换
来源：http://fhb.zhaomingkeji.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qxq.cqqwz.cn

[R24] 大小写转换
来源：http://fbg.yfazqb.com

echo "${s^^}"; echo "${s,,}"
来源：http://btk.uphjek.com

[R25] 去后缀 / 去前缀
来源：http://uey.wangshuangyany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ebn.haohaochexian.top

[R26] 命令替换
来源：http://qib.jqgfzy.top

now=$(date +%F); echo "$now"
来源：http://hvl.aizwys.cn

[R27] 算术展开
来源：http://tci.nwbrower.top

echo $((1 + 2 * 3))
来源：http://rgk.zdbjq.cn

[R28] 浮点运算
来源：http://zwd.zhongyouzk.top

echo "scale=2; 10/3" | bc
来源：http://xzz.xuetiantiany.cn

[R29] 定义函数
来源：http://gdq.ydjk.org.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mpd.vqdsnc.cn

[R30] 函数返回状态码
来源：http://oyn.yueranfly.top

f() { return 0; }; f || echo "失败了"
来源：http://ofr.gotoacloud.top

[R31] 局部变量
来源：http://car.yj202588.top

f() { local x=1; echo "$x"; }
来源：http://fei.hesvh.cn

[R32] 参数个数校验
来源：http://ksd.yvedp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jvi.gzhubu.top

[R33] 捕获错误并提示行号
来源：http://gqx.yuanzhike.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://whs.haohaochexian.top

[R34] 退出时清理
来源：http://ime.shanyushiyangtech.top

trap 'rm -f "$tmp"' EXIT
来源：http://zxn.nwbrower.top

[R35] 后台执行并等待
来源：http://txw.aibaodan.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wbi.yuxming.cn

[R36] 并发执行多个任务
来源：http://hhg.ybcxt.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jrk.xinyue.icu

[R37] 把输出赋给变量
来源：http://wnu.zdbjq.cn

files=$(ls -1)
来源：http://xrc.ydzc1.top

[R38] 管道串联
来源：http://oyq.jqgufenzy.top

cat a.txt | grep -i error | wc -l
来源：http://jwd.hammf.cn

[R39] 重定向标准输出与错误
来源：http://bqv.jianghu66.top

cmd > out.log 2>&1
来源：http://hbo.zhiwuduotai.top

[R40] 追加写日志
来源：http://tkm.sufxvd.cn

echo "log" >> out.log
来源：http://qxa.yfazqb.com

[R41] 丢弃输出
来源：http://jzc.xingfuxueyuan.xyz

cmd >/dev/null 2>&1
来源：http://wkb.shangyingyoupin.top

[R42] 输入重定向
来源：http://viv.jianghu66.top

wc -l < a.txt
来源：http://ncv.shanyushiyangkeji.top

[R43] 按名字查找文件
来源：http://nnx.hfpthk.cn

find . -name "*.log" -type f
来源：http://omr.zhiwuduotai.top

[R44] 按修改时间查找
来源：http://mhf.zdqjudy.top

find . -mtime -7 -type f
来源：http://hyh.vehdjk.com

[R45] 批量删除
来源：http://dti.sxryk.cn

find . -name "*.tmp" -delete
来源：http://qrf.yfazqb.com

[R46] 递归替换文件内容
来源：http://nzh.fehbvm.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://unm.tian-w.cn

[R47] sed 单行替换
来源：http://nzy.shzxlz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dbr.pengpengdd.cyou

[R48] awk 取指定列
来源：http://mkb.ctjpmb.com

awk '{print $1, $3}' a.txt
来源：http://qll.cqqwz.cn

[R49] awk 带条件
来源：http://dhs.zdbjq.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://otn.yonumen.top

[R50] awk 求和
来源：http://rmk.haohaochexian.top

awk '{s += $2} END {print s}' a.txt
来源：http://yoc.shangyingyoupin.top

[R51] 排序去重取前几
来源：http://rce.feifeiyinyue.top

sort a.txt | uniq -c | sort -rn | head
来源：http://tuo.ybcxt.top

[R52] 统计行数
来源：http://fex.chenzaomai.com

wc -l a.txt
来源：http://qjb.sxryk.cn

[R53] 查看文件头与实时尾
来源：http://mqs.yuxming.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zki.haohaochexian.top

[R54] 比较两个文件
来源：http://spx.aibaodan.cn

diff a.txt b.txt
来源：http://qxk.ehwqpu.com

[R55] 压缩与解压
来源：http://mir.fzhhl.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ukf.yj20258.top

[R56] 远程拷贝
来源：http://haj.hysaishi.cn

scp file user@host:/path/
来源：http://chr.hnqzz.top

[R57] 远程执行命令
来源：http://wlg.nanxinkj.top

ssh user@host 'uptime'
来源：http://fgr.svipenyu.cn

[R58] 下载文件
来源：http://cul.cdnleiting.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yjo.shangyingyoupin.top

[R59] 发 POST JSON
来源：http://gmh.hesvh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ceq.nwbrower.top

[R60] 只看 HTTP 状态码
来源：http://kbb.hesvh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nfv.kuanghao11.cn

[R61] 磁盘占用
来源：http://rge.fanxiaobao.xyz

df -h;  du -sh *
来源：http://tee.yfazqb.com

[R62] 找最占空间的文件
来源：http://qbc.tanke756.top

du -ah . | sort -rh | head -10
来源：http://lhz.gotoacloud.top

[R63] 内存与进程
来源：http://uov.yongpay.top

free -h;  ps aux | grep nginx
来源：http://gtp.gzhubu.top

[R64] 结束进程
来源：http://yqv.nanxinkj.top

kill -9 $(pgrep -f app.py)
来源：http://acv.quarkkingdee.top

[R65] 查看端口占用
来源：http://jzo.hesvh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fss.daria6918.cn

[R66] 定时任务
来源：http://itk.yj20258.top

crontab -e;  crontab -l
来源：http://vft.gotoacloud.top

[R67] 生成随机十六进制串
来源：http://vum.jinghuilouyu.cn

openssl rand -hex 16
来源：http://jim.redwolf501.top

[R68] 计算文件校验值
来源：http://bxw.feifeiyinyue.top

sha256sum a.txt;  md5sum a.txt
来源：http://shn.xylfe.cn

[R69] 生成随机密码
来源：http://hbk.mhx1999.top

head -c 16 /dev/urandom | base64
来源：http://nvj.tianlin.xyz

[R70] 时间戳与互转
来源：http://xht.ybcxt.top

date +%s;  date -d @1700000000
来源：http://bng.hysaishi.cn

[R71] 日期格式化
来源：http://ohs.xingfuxueyuan.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://jda.aizwys.cn

[R72] 等待端口就绪
来源：http://ndx.ywan-chungtsiang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://xot.cqqwz.cn

[R73] 分割大日志
来源：http://ytx.fzhhl.top

split -l 1000 big.log part_
来源：http://lgm.hysaishi.cn

[R74] 批量重命名
来源：http://fio.ivvv.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fuf.sxryk.cn

[R75] 导出环境变量
来源：http://rvi.ywan-chungtsiang.top

export PATH="$HOME/bin:$PATH"
来源：http://ytz.jinghuilouyu.cn

[R76] 使用临时文件
来源：http://uhu.uphjek.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wae.shzxlz.cn

[R77] 读取用户输入
来源：http://dcc.jyoumei.cn

read -rp "请输入: " ans
来源：http://ziv.cheryme.top

[R78] 交互式菜单
来源：http://kxa.jinyuanbaomall.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://suh.yj202588.top

[R79] 解析命令行选项
来源：http://iug.tarul.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ira.xuetiantiany.cn

[R80] 查看脚本执行耗时
来源：http://wmu.316326.xyz

time ./run.sh
来源：http://yse.chenlongwang.top

================================================================================
来源：http://efg.ywan-chungtsiang.top

S. C / C++ 专题
来源：http://sqn.fehbvm.com

================================================================================
来源：http://xaw.guannengcc.top

[S01] C：Hello World
来源：http://dau.yvedp.cn

#include <stdio.h>
来源：http://vve.cqqwz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://got.daria6918.cn

[S02] C：变量与格式化输出
来源：http://itf.zdqjudy.top

int a = 10; printf("%d\n", a);
来源：http://jjx.redwolf501.top

[S03] C：读入整数
来源：http://btr.ydjk.org.cn

int x; scanf("%d", &x);
来源：http://jao.zhaomingkeji.xyz

[S04] C：字符串复制
来源：http://sfr.nanxuanxn.top

char dst[32]; strcpy(dst, "hi");
来源：http://yqa.yuxming.cn

[S05] C：字符串长度
来源：http://frp.gogol.net.cn

strlen(s)
来源：http://szw.jinyuanbaomall.cn

[S06] C：字符串比较
来源：http://lzl.tanke756.top

strcmp(a, b) == 0
来源：http://ans.zhijiandao.cn

[S07] C：数组遍历求和
来源：http://hni.xuetiantiany.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cik.tianlin.xyz

[S08] C：动态内存分配与释放
来源：http://sia.nwbrower.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lqo.c1oappe.top

[S09] C：结构体定义与初始化
来源：http://wge.hnxiangtu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pjx.yj202588.top

[S10] C：指针与解引用
来源：http://jip.zdbjq.cn

int *p = &a;  *p = 5;
来源：http://pxn.sjlbkw.cn

[S11] C：逐行读文件
来源：http://jyp.snrcjt.cn

FILE *f = fopen("a.txt", "r");
来源：http://eot.xuetiantiany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yhc.svipenyu.cn

fclose(f);
来源：http://ygq.jyoumei.cn

[S12] C：写文件
来源：http://blt.zhoulong.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pnw.yuanzhike.top

[S13] C：宏定义
来源：http://utz.tian-w.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hfv.zhongyouzk.top

[S14] C：枚举
来源：http://ohp.tanke756.top

enum Color { RED, GREEN, BLUE };
来源：http://unj.fengsongda.top

[S15] C：类型转换
来源：http://scd.gogol.net.cn

(double) a / b
来源：http://gsj.yuanzhike.top

[S16] C：位操作置位
来源：http://eie.hnxiangtu.top

x |= (1 << 3);
来源：http://oha.birdmap.top

[S17] C：安全拼接字符串
来源：http://hei.yanxiufei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sya.yj202588.top

[S18] C：命令行参数
来源：http://wec.yonumen.top

int main(int argc, char **argv)
来源：http://skq.snrcjt.cn

[S19] C：快速排序
来源：http://fnl.chenlongwang.top

qsort(a, n, sizeof(int), cmp);
来源：http://lve.yangfankeji.com

[S20] C：二分查找
来源：http://bra.epnwcf.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ual.smart0.xyz

[S21] C：字符类别判断
来源：http://ktv.52xcode.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xyh.redwolf501.top

[S22] C：字符串转数字
来源：http://ihx.vehdjk.com

atoi("42");  strtod("3.14", NULL);
来源：http://hom.zdbjq.cn

[S23] C：随机数
来源：http://agu.yj20258.top

srand(time(NULL));  int r = rand() % 100;
来源：http://sgf.cqqwz.cn

[S24] C：获取本地时间
来源：http://xng.birdmap.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qhq.quarkkingdee.top

[S25] C：内存拷贝
来源：http://mnu.mhx1999.top

memcpy(dst, src, n);
来源：http://bpn.kuanghao11.cn

[S26] C：内存清零
来源：http://hzw.daxiang520.top

memset(a, 0, sizeof a);
来源：http://gan.xinyue.icu

[S27] C：定义常量
来源：http://zyj.hongshengwenyu.top

const double PI = 3.14159;
来源：http://oqa.nwbrower.top

[S28] C：静态变量
来源：http://fig.gotoacloud.top

static int counter = 0;
来源：http://yoc.xylfe.cn

[S29] C：变参函数
来源：http://qud.quarkkingdee.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://byj.ppjwa.cn

[S30] C：头文件保护
来源：http://ojt.ydjk.org.cn

#ifndef X_H
来源：http://rmj.chenjidiqi.icu

#define X_H
来源：http://rto.smart0.xyz

#endif
来源：http://ame.nanxinkj.top

[S31] C++：Hello World
来源：http://xlb.xuetiantiany.cn

#include <iostream>
来源：http://fuc.ctjpmb.com

int main() { std::cout << "Hello\n"; }
来源：http://hxq.xuanzx.com

[S32] C++：字符串
来源：http://abq.9152youxi.cn

std::string s = "hi";  s += "!";
来源：http://dbm.jlsjyb.cn

[S33] C++：vector 增删
来源：http://qoy.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://njj.xziqi.cn

[S34] C++：遍历 vector
来源：http://ssk.ydzc1.top

for (auto &x : v) { std::cout << x; }
来源：http://yud.iojbl.cn

[S35] C++：map
来源：http://izf.zhixingplan.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zhd.snrcjt.cn

[S36] C++：unordered_map
来源：http://nfi.yj20258.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sah.feifeiyinyue.top

[S37] C++：set
来源：http://ulz.sweek.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ejq.ywan-chungtsiang.top

[S38] C++：排序
来源：http://szi.shangyingyoupin.top

std::sort(v.begin(), v.end());
来源：http://myo.zhixingplan.top

[S39] C++：自定义比较器排序
来源：http://uvc.haohaochexian.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tbm.ydjk.org.cn

[S40] C++：查找元素
来源：http://sas.zhiwuduotai.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lsf.fanxiaobao.xyz

[S41] C++：类与构造函数
来源：http://nej.nwbrower.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://omz.jiagoushi.top

[S42] C++：继承与虚函数
来源：http://qzr.shuidangran.top

class B : public Base { public: void f() override {} };
来源：http://zni.aibaodan.cn

[S43] C++：智能指针
来源：http://pbu.hnxiangtu.top

auto p = std::make_unique<int>(5);
来源：http://pfg.fzhhl.top

[S44] C++：引用传参
来源：http://tuj.ydzc1.top

void inc(int &x) { ++x; }
来源：http://rgv.bbcook.cn

[S45] C++：lambda
来源：http://lbb.sjlbkw.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tvc.guowangkeji.top

[S46] C++：函数模板
来源：http://vbb.birdmap.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jow.tian-w.cn

[S47] C++：结构化绑定遍历
来源：http://bpq.redwolf501.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oym.havefunace.top

[S48] C++：逐行读文件
来源：http://kyp.jlsjyb.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vre.hywenlv.cn

while (std::getline(in, line)) { }
来源：http://yrg.hammf.cn

[S49] C++：写文件
来源：http://ljw.tianlin.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jnc.epnwcf.com

[S50] C++：格式化数字
来源：http://kiw.zhoulong.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vrs.pycfn.com

[S51] C++：显式类型转换
来源：http://lbk.pycfn.com

static_cast<double>(a) / b
来源：http://wsa.fzhhl.top

[S52] C++：const 与 noexcept
来源：http://vnd.zhengqikj.top

int size() const noexcept { return n_; }
来源：http://jau.tanke756.top

[S53] C++：移动语义
来源：http://dqb.ppjwa.cn

std::vector<int> w = std::move(v);
来源：http://shh.hnqzz.top

[S54] C++：异常处理
来源：http://ylc.shanyushiyangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lfv.redwolf501.top

[S55] C++：结构化绑定
来源：http://mst.hongshengwenyu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jhz.jinqigufen.top

[S56] C++：optional
来源：http://riz.yfazqb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qvz.gzhubu.top

[S57] C++：编译期常量
来源：http://ecz.fengsongda.top

constexpr int N = 10;
来源：http://tzn.yongpay.top

[S58] C++：命名空间
来源：http://zhk.shzxlz.cn

namespace ns { int f() { return 1; } }
来源：http://ehn.gaohongyu789.top

[S59] C++：静态断言
来源：http://zwp.aibaodan.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ede.shuidangran.top

[S60] C++：遍历并删除元素
来源：http://asy.ydzc1.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ofq.sysykeji.top

================================================================================
来源：http://umn.xylfe.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eyn.ybcxt.top

================================================================================
来源：http://att.yj202588.top

[T01] Kotlin：Hello World
来源：http://vge.feifeiyinyue.top

println("Hello")
来源：http://gkh.zhaomingkeji.xyz

[T02] Kotlin：变量
来源：http://jna.sxryk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xur.yj20258.top

[T03] Kotlin：字符串模板
来源：http://tzc.cashguo.top

"值: $b"
来源：http://gyg.gzhubu.top

[T04] Kotlin：空安全
来源：http://veh.mhx1999.top

val n: String? = null;  n?.length
来源：http://ezk.yueranfly.top

[T05] Kotlin：when 表达式
来源：http://xoc.hfpthk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lgk.yvedp.cn

[T06] Kotlin：集合映射
来源：http://xgc.wangshuangyany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fmz.smart0.xyz

[T07] Kotlin：集合过滤
来源：http://uzv.316326.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://niv.bjfxy.top

[T08] Kotlin：数据类
来源：http://mma.yj20258.top

data class User(val name: String, val age: Int)
来源：http://xsq.ydzc1.top

[T09] Kotlin：扩展函数
来源：http://fvu.tianlin.xyz

fun String.exclaim() = this + "!"
来源：http://sgt.xuanzx.com

[T10] Kotlin：默认参数
来源：http://fer.yanxiufei.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nni.epnwcf.com

[T11] Kotlin：协程
来源：http://sea.zhiwuduotai.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hqm.ydzc1.top

[T12] Kotlin：解构声明
来源：http://hia.shangyingyoupin.top

val (a, b) = Pair(1, 2)
来源：http://fxp.yvedp.cn

[T13] Kotlin：只读 Map
来源：http://plr.vehdjk.com

val m = mapOf("a" to 1)
来源：http://gzd.chenzaomai.com

[T14] Kotlin：循环
来源：http://ejh.cqqwz.cn

for (i in 1..10) println(i)
来源：http://cyf.jinqigufen.top

[T15] Kotlin：接口
来源：http://ibu.uphjek.com

interface Shape { fun area(): Double }
来源：http://gvu.jyoumei.cn

[T16] Swift：Hello World
来源：http://fmi.chenlongwang.top

print("Hello")
来源：http://hwl.zhiwuduotai.top

[T17] Swift：变量与常量
来源：http://vji.c1oappe.top

var a = 1;  let b = 2
来源：http://sva.yj20258888.top

[T18] Swift：字符串插值
来源：http://kuh.316326.xyz

"值: \(b)"
来源：http://njy.chenzaomai.com

[T19] Swift：可选绑定
来源：http://hwm.tarul.cn

if let n = opt { print(n) }
来源：http://zdx.ctjpmb.com

[T20] Swift：数组操作
来源：http://dfy.chenlongwang.top

var a = [1, 2, 3];  a.append(4)
来源：http://uks.yvedp.cn


<!-- 参考信息 -->