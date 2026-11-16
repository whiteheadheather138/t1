代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://frg.bbcook.cn

[R16] until 等待条件
来源：http://gvf.redwolf501.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xyu.hysaishi.cn

[R17] 数组定义与取值
来源：http://ztv.hongshengwenyu.top

arr=(a b c); echo "${arr[0]}"
来源：http://ihq.pengpengdd.cyou

[R18] 遍历数组
来源：http://xwx.ywan-chungtsiang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bcs.hnxiangtu.top

[R19] 数组长度
来源：http://pmy.hcnkem.com

echo "${#arr[@]}"
来源：http://ttq.xziqi.cn

[R20] 关联数组（字典）
来源：http://ixq.cucudq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vqf.xuetiantiany.cn

[R21] 字符串长度
来源：http://jub.0kj1m.cn

echo "${#s}"
来源：http://yoj.hfpthk.cn

[R22] 截取子串
来源：http://jtm.bbcook.cn

echo "${s:0:5}"
来源：http://xkv.ybcxt.top

[R23] 字符串替换
来源：http://aqg.sweek.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qkq.yueranfly.top

[R24] 大小写转换
来源：http://dhe.hammf.cn

echo "${s^^}"; echo "${s,,}"
来源：http://van.hesvh.cn

[R25] 去后缀 / 去前缀
来源：http://wpi.hesvh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xlf.yfazqb.com

[R26] 命令替换
来源：http://rxz.hywenlv.cn

now=$(date +%F); echo "$now"
来源：http://ugt.hysaishi.cn

[R27] 算术展开
来源：http://ece.hammf.cn

echo $((1 + 2 * 3))
来源：http://fgb.gaohongyu789.top

[R28] 浮点运算
来源：http://kqq.svipenyu.cn

echo "scale=2; 10/3" | bc
来源：http://vse.52xcode.cn

[R29] 定义函数
来源：http://fcu.aibaodan.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zab.tanke756.top

[R30] 函数返回状态码
来源：http://uuy.ctjpmb.com

f() { return 0; }; f || echo "失败了"
来源：http://vyz.vqdsnc.cn

[R31] 局部变量
来源：http://tfh.yvedp.cn

f() { local x=1; echo "$x"; }
来源：http://mur.hnqzz.top

[R32] 参数个数校验
来源：http://oln.316326.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xkk.hysaishi.cn

[R33] 捕获错误并提示行号
来源：http://xfx.gaohongyu789.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yoh.chenjidiqi.icu

[R34] 退出时清理
来源：http://nhl.bbcook.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tuu.jinghuilouyu.cn

[R35] 后台执行并等待
来源：http://paj.nwbrower.top

sleep 5 & pid=$!; wait "$pid"
来源：http://cad.chenzaomai.com

[R36] 并发执行多个任务
来源：http://jtx.sysykeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hkf.yangfankeji.com

[R37] 把输出赋给变量
来源：http://tcb.aizwys.cn

files=$(ls -1)
来源：http://qdg.ppjwa.cn

[R38] 管道串联
来源：http://itg.jinqigufen.top

cat a.txt | grep -i error | wc -l
来源：http://dnf.tanke756.top

[R39] 重定向标准输出与错误
来源：http://esu.dashuyun.cn

cmd > out.log 2>&1
来源：http://lbf.xinyue.icu

[R40] 追加写日志
来源：http://hng.bjfxy.top

echo "log" >> out.log
来源：http://yxs.ywan-chungtsiang.top

[R41] 丢弃输出
来源：http://ggk.gotoacloud.top

cmd >/dev/null 2>&1
来源：http://vio.jqgufenzy.top

[R42] 输入重定向
来源：http://tpw.nanxinkj.top

wc -l < a.txt
来源：http://zht.shuidangran.top

[R43] 按名字查找文件
来源：http://zpr.xylfe.cn

find . -name "*.log" -type f
来源：http://hzh.yangfankeji.com

[R44] 按修改时间查找
来源：http://pac.vqdsnc.cn

find . -mtime -7 -type f
来源：http://beg.yfazqb.com

[R45] 批量删除
来源：http://eik.bjfxy.top

find . -name "*.tmp" -delete
来源：http://pcy.ehwqpu.com

[R46] 递归替换文件内容
来源：http://duo.aizwys.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://trj.ppjwa.cn

[R47] sed 单行替换
来源：http://msh.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://jlf.ydjk.org.cn

[R48] awk 取指定列
来源：http://voi.vehdjk.com

awk '{print $1, $3}' a.txt
来源：http://xat.pycfn.com

[R49] awk 带条件
来源：http://ujx.uphjek.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cog.quarkkingdee.top

[R50] awk 求和
来源：http://flh.guowangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://jhm.epnwcf.com

[R51] 排序去重取前几
来源：http://rpy.ybcxt.top

sort a.txt | uniq -c | sort -rn | head
来源：http://wmi.ybcxt.top

[R52] 统计行数
来源：http://gnf.yueranfly.top

wc -l a.txt
来源：http://ttl.gogol.net.cn

[R53] 查看文件头与实时尾
来源：http://bvn.hfpthk.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wvd.nwbrower.top

[R54] 比较两个文件
来源：http://fco.aizwys.cn

diff a.txt b.txt
来源：http://zvb.tian-w.cn

[R55] 压缩与解压
来源：http://ujt.xingfuxueyuan.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vex.hongshengwenyu.top

[R56] 远程拷贝
来源：http://pzz.pengpengdd.cyou

scp file user@host:/path/
来源：http://tvl.cdnleiting.top

[R57] 远程执行命令
来源：http://suh.iojbl.cn

ssh user@host 'uptime'
来源：http://ban.316326.xyz

[R58] 下载文件
来源：http://opu.ivvv.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dfn.cashguo.top

[R59] 发 POST JSON
来源：http://dlz.shuidangran.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bir.yonumen.top

[R60] 只看 HTTP 状态码
来源：http://och.xziqi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fzt.tanke756.top

[R61] 磁盘占用
来源：http://txb.xziqi.cn

df -h;  du -sh *
来源：http://fmu.zhaomingkeji.xyz

[R62] 找最占空间的文件
来源：http://hhk.hysaishi.cn

du -ah . | sort -rh | head -10
来源：http://skq.9152youxi.cn

[R63] 内存与进程
来源：http://kau.gzhubu.top

free -h;  ps aux | grep nginx
来源：http://nnt.fengsongda.top

[R64] 结束进程
来源：http://voj.yvedp.cn

kill -9 $(pgrep -f app.py)
来源：http://xsq.tian-w.cn

[R65] 查看端口占用
来源：http://txu.xuetiantiany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xsl.haohaochexian.top

[R66] 定时任务
来源：http://jmr.yuanzhike.top

crontab -e;  crontab -l
来源：http://lrx.yvedp.cn

[R67] 生成随机十六进制串
来源：http://odg.yonumen.top

openssl rand -hex 16
来源：http://kqz.yj202588.top

[R68] 计算文件校验值
来源：http://siv.shanyushiyangkeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://tqq.daria6918.cn

[R69] 生成随机密码
来源：http://aah.kuanghao11.cn

head -c 16 /dev/urandom | base64
来源：http://ryu.shuidangran.top

[R70] 时间戳与互转
来源：http://ghu.quarkkingdee.top

date +%s;  date -d @1700000000
来源：http://kim.zycfv.cn

[R71] 日期格式化
来源：http://qdz.ctjpmb.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://hlp.jqgfzy.top

[R72] 等待端口就绪
来源：http://iqo.jiagoushi.top

until nc -z localhost 3306; do sleep 1; done
来源：http://yqg.xinyue.icu

[R73] 分割大日志
来源：http://iem.wangshuangyany.cn

split -l 1000 big.log part_
来源：http://auz.dashuyun.cn

[R74] 批量重命名
来源：http://nwn.shzxlz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uwu.daxiang520.top

[R75] 导出环境变量
来源：http://qsf.yonumen.top

export PATH="$HOME/bin:$PATH"
来源：http://vmx.sysykeji.top

[R76] 使用临时文件
来源：http://ubg.yuxming.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lae.ivvv.top

[R77] 读取用户输入
来源：http://ume.andypj.xyz

read -rp "请输入: " ans
来源：http://rvn.jinqigufen.top

[R78] 交互式菜单
来源：http://zco.hnqzz.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jgl.shanyushiyangtech.top

[R79] 解析命令行选项
来源：http://pqi.feifeiyinyue.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hjj.cheryme.top

[R80] 查看脚本执行耗时
来源：http://mog.xziqi.cn

time ./run.sh
来源：http://apw.yuxming.cn

================================================================================
来源：http://nxv.smart0.xyz

S. C / C++ 专题
来源：http://knv.dianchejie.cn

================================================================================
来源：http://btg.xylfe.cn

[S01] C：Hello World
来源：http://iqe.sjlbkw.cn

#include <stdio.h>
来源：http://cvs.cashguo.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://chj.hywenlv.cn

[S02] C：变量与格式化输出
来源：http://crv.zhaomingkeji.xyz

int a = 10; printf("%d\n", a);
来源：http://idr.tarul.cn

[S03] C：读入整数
来源：http://eyh.shangyingyoupin.top

int x; scanf("%d", &x);
来源：http://enr.chenjidiqi.icu

[S04] C：字符串复制
来源：http://ron.hysaishi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yjh.shanyushiyangkeji.top

[S05] C：字符串长度
来源：http://duw.sufxvd.cn

strlen(s)
来源：http://xaw.tarul.cn

[S06] C：字符串比较
来源：http://rut.havefunace.top

strcmp(a, b) == 0
来源：http://nig.iojbl.cn

[S07] C：数组遍历求和
来源：http://xhh.yonumen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://itj.dianchejie.cn

[S08] C：动态内存分配与释放
来源：http://cpz.feifeiyinyue.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://imb.hnqzz.top

[S09] C：结构体定义与初始化
来源：http://gxp.xingfuxueyuan.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xxl.smart0.xyz

[S10] C：指针与解引用
来源：http://qto.wangdashe.top

int *p = &a;  *p = 5;
来源：http://xix.sufxvd.cn

[S11] C：逐行读文件
来源：http://kqc.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://pvn.hnqzz.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://eym.fktsv.cn

fclose(f);
来源：http://jiq.hnxiangtu.top

[S12] C：写文件
来源：http://hqa.jyoumei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ddi.daria6918.cn

[S13] C：宏定义
来源：http://ncg.gotoacloud.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qjg.fzhhl.top

[S14] C：枚举
来源：http://kap.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://ogc.zdqjudy.top

[S15] C：类型转换
来源：http://znq.jlsjyb.cn

(double) a / b
来源：http://zsr.kuanghao11.cn

[S16] C：位操作置位
来源：http://zbz.pycfn.com

x |= (1 << 3);
来源：http://kyd.tian-w.cn

[S17] C：安全拼接字符串
来源：http://waw.andypj.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://crx.kuanghao11.cn

[S18] C：命令行参数
来源：http://nkd.svipenyu.cn

int main(int argc, char **argv)
来源：http://une.cashguo.top

[S19] C：快速排序
来源：http://olb.aibaodan.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xpl.tanke756.top

[S20] C：二分查找
来源：http://mqt.yuanzhike.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://red.ivvv.top

[S21] C：字符类别判断
来源：http://gqh.yuxming.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zpw.sufxvd.cn

[S22] C：字符串转数字
来源：http://nnl.svipenyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oyp.ppjwa.cn

[S23] C：随机数
来源：http://oxg.zdqjudy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://cik.316326.xyz

[S24] C：获取本地时间
来源：http://ofx.mhx1999.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nsi.zhiwuduotai.top

[S25] C：内存拷贝
来源：http://yrc.jiagoushi.top

memcpy(dst, src, n);
来源：http://ukj.jlsjyb.cn

[S26] C：内存清零
来源：http://rzc.jinqigfzy.top

memset(a, 0, sizeof a);
来源：http://ysu.sjlbkw.cn

[S27] C：定义常量
来源：http://tgz.hnqzz.top

const double PI = 3.14159;
来源：http://lab.ctjpmb.com

[S28] C：静态变量
来源：http://qxo.bjfxy.top

static int counter = 0;
来源：http://nis.redwolf501.top

[S29] C：变参函数
来源：http://dik.daxiang520.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ynl.zdqjudy.top

[S30] C：头文件保护
来源：http://tvm.yuxming.cn

#ifndef X_H
来源：http://kjf.xinyue.icu

#define X_H
来源：http://quk.dashuyun.cn

#endif
来源：http://mer.wangdashe.top

[S31] C++：Hello World
来源：http://tqt.hammf.cn

#include <iostream>
来源：http://lxr.pengpengdd.cyou

int main() { std::cout << "Hello\n"; }
来源：http://lep.ivvv.top

[S32] C++：字符串
来源：http://kbq.guannengcc.top

std::string s = "hi";  s += "!";
来源：http://yka.sjlbkw.cn

[S33] C++：vector 增删
来源：http://lxq.xinyue.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uil.wangdashe.top

[S34] C++：遍历 vector
来源：http://uku.yueranfly.top

for (auto &x : v) { std::cout << x; }
来源：http://rba.smart0.xyz

[S35] C++：map
来源：http://tgi.chenzaomai.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mfa.dianchejie.cn

[S36] C++：unordered_map
来源：http://cin.chenjidiqi.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wfw.jiagoushi.top

[S37] C++：set
来源：http://itg.xinyue.icu

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cdi.bjfxy.top

[S38] C++：排序
来源：http://wcx.ppjwa.cn

std::sort(v.begin(), v.end());
来源：http://oyc.cashguo.top

[S39] C++：自定义比较器排序
来源：http://jpm.redwolf501.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tfq.xuetiantiany.cn

[S40] C++：查找元素
来源：http://bjs.0kj1m.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fgn.quarkkingdee.top

[S41] C++：类与构造函数
来源：http://yvk.ctjpmb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mrm.xuanzx.com

[S42] C++：继承与虚函数
来源：http://mvt.jinyuanbaomall.cn

class B : public Base { public: void f() override {} };
来源：http://epn.yj20258.top

[S43] C++：智能指针
来源：http://bfw.zhiwuduotai.top

auto p = std::make_unique<int>(5);
来源：http://jah.dashuyun.cn

[S44] C++：引用传参
来源：http://hrj.iojbl.cn

void inc(int &x) { ++x; }
来源：http://kcu.aibaodan.cn

[S45] C++：lambda
来源：http://rbt.snrcjt.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ewz.ywan-chungtsiang.top

[S46] C++：函数模板
来源：http://iro.hesvh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://iao.hnxiangtu.top

[S47] C++：结构化绑定遍历
来源：http://bki.fehbvm.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lxt.redwolf501.top

[S48] C++：逐行读文件
来源：http://bvl.yj20258.top

std::ifstream in("a.txt");  std::string line;
来源：http://hiy.fzhhl.top

while (std::getline(in, line)) { }
来源：http://ojc.gogol.net.cn

[S49] C++：写文件
来源：http://dec.xylfe.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qpe.jyoumei.cn

[S50] C++：格式化数字
来源：http://pdl.sweek.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iuc.yongpay.top

[S51] C++：显式类型转换
来源：http://yqf.hywenlv.cn

static_cast<double>(a) / b
来源：http://mqw.dianchejie.cn

[S52] C++：const 与 noexcept
来源：http://cpy.zhixingplan.top

int size() const noexcept { return n_; }
来源：http://zrq.jinyuanbaomall.cn

[S53] C++：移动语义
来源：http://bdx.jinyuanbaomall.cn

std::vector<int> w = std::move(v);
来源：http://fcn.dashuyun.cn

[S54] C++：异常处理
来源：http://gle.dashuyun.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zbq.tianlin.xyz

[S55] C++：结构化绑定
来源：http://asx.snrcjt.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vml.jyoumei.cn

[S56] C++：optional
来源：http://vaa.daxiang520.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ikp.ybcxt.top

[S57] C++：编译期常量
来源：http://pre.hesvh.cn

constexpr int N = 10;
来源：http://zhz.zhijiandao.cn

[S58] C++：命名空间
来源：http://dtb.yj20258888.top

namespace ns { int f() { return 1; } }
来源：http://kvs.uphjek.com

[S59] C++：静态断言
来源：http://ecz.guannengcc.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kvn.jinghuilouyu.cn

[S60] C++：遍历并删除元素
来源：http://dxj.chenzaomai.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lsv.zdbjq.cn

================================================================================
来源：http://ycw.guowangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kqr.uphjek.com

================================================================================
来源：http://mls.cdnleiting.top

[T01] Kotlin：Hello World
来源：http://qwa.nanxinkj.top

println("Hello")
来源：http://uor.hcnkem.com

[T02] Kotlin：变量
来源：http://jwv.jinghuilouyu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dvp.xuanzx.com

[T03] Kotlin：字符串模板
来源：http://dyt.jinyuanbaomall.cn

"值: $b"
来源：http://qyk.chenlongwang.top

[T04] Kotlin：空安全
来源：http://fao.yonumen.top

val n: String? = null;  n?.length
来源：http://wnt.shangyingyoupin.top

[T05] Kotlin：when 表达式
来源：http://djm.sysykeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rhy.jqgufenzy.top

[T06] Kotlin：集合映射
来源：http://upb.guowangkeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://oeb.quarkkingdee.top

[T07] Kotlin：集合过滤
来源：http://jex.bjfxy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://iec.9152youxi.cn

[T08] Kotlin：数据类
来源：http://amr.nwbrower.top

data class User(val name: String, val age: Int)
来源：http://snd.daxiang520.top

[T09] Kotlin：扩展函数
来源：http://jun.yfazqb.com

fun String.exclaim() = this + "!"
来源：http://chn.jinqigufen.top

[T10] Kotlin：默认参数
来源：http://vyf.kuanghao11.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lat.cucudq.cn

[T11] Kotlin：协程
来源：http://ufu.hesvh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://igo.feifeiyinyue.top

[T12] Kotlin：解构声明
来源：http://phz.hfpthk.cn

val (a, b) = Pair(1, 2)
来源：http://hdx.iojbl.cn

[T13] Kotlin：只读 Map
来源：http://cac.nanxuanxn.top

val m = mapOf("a" to 1)
来源：http://yqv.gzhubu.top

[T14] Kotlin：循环
来源：http://tou.fanxiaobao.xyz

for (i in 1..10) println(i)
来源：http://uda.jianghu66.top

[T15] Kotlin：接口
来源：http://dzh.gotoacloud.top

interface Shape { fun area(): Double }
来源：http://jcp.yuxming.cn

[T16] Swift：Hello World
来源：http://xuu.yj202588.top

print("Hello")
来源：http://fnc.zdqjudy.top

[T17] Swift：变量与常量
来源：http://frf.daxiang520.top

var a = 1;  let b = 2
来源：http://nsd.xinyue.icu

[T18] Swift：字符串插值
来源：http://ptn.vqdsnc.cn

"值: \(b)"
来源：http://yne.nanxinkj.top


<!-- 参考信息 -->