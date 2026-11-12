代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qyk.guannengcc.top

[R16] until 等待条件
来源：http://fol.gzhubu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bpn.wangshuangyany.cn

[R17] 数组定义与取值
来源：http://riz.sufxvd.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kis.wangshuangyany.cn

[R18] 遍历数组
来源：http://gpq.jinqigfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sdr.zdbjq.cn

[R19] 数组长度
来源：http://unb.iojbl.cn

echo "${#arr[@]}"
来源：http://she.gzhubu.top

[R20] 关联数组（字典）
来源：http://rce.jinghuilouyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yoa.hysaishi.cn

[R21] 字符串长度
来源：http://ttf.hnqzz.top

echo "${#s}"
来源：http://wts.jqgufenzy.top

[R22] 截取子串
来源：http://sfh.ctjpmb.com

echo "${s:0:5}"
来源：http://myf.yueranfly.top

[R23] 字符串替换
来源：http://poy.vehdjk.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lep.52xcode.cn

[R24] 大小写转换
来源：http://qnr.feifeiyinyue.top

echo "${s^^}"; echo "${s,,}"
来源：http://pon.yangfankeji.com

[R25] 去后缀 / 去前缀
来源：http://wmn.daxiang520.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://oul.svipenyu.cn

[R26] 命令替换
来源：http://szj.yj20258.top

now=$(date +%F); echo "$now"
来源：http://ptg.haohaochexian.top

[R27] 算术展开
来源：http://qps.cheryme.top

echo $((1 + 2 * 3))
来源：http://pkl.zhijiandao.cn

[R28] 浮点运算
来源：http://xah.hfpthk.cn

echo "scale=2; 10/3" | bc
来源：http://hei.jinyuanbaomall.cn

[R29] 定义函数
来源：http://rrl.zhaomingkeji.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lxb.guowangkeji.top

[R30] 函数返回状态码
来源：http://dkb.epnwcf.com

f() { return 0; }; f || echo "失败了"
来源：http://tom.yuanzhike.top

[R31] 局部变量
来源：http://ncb.jqgufenzy.top

f() { local x=1; echo "$x"; }
来源：http://atb.yongpay.top

[R32] 参数个数校验
来源：http://xnu.zycfv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nqv.yonumen.top

[R33] 捕获错误并提示行号
来源：http://jcp.shanyushiyangtech.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pau.xuetiantiany.cn

[R34] 退出时清理
来源：http://wbk.sjlbkw.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pnk.jqgufenzy.top

[R35] 后台执行并等待
来源：http://tae.yueranfly.top

sleep 5 & pid=$!; wait "$pid"
来源：http://szj.dianchejie.cn

[R36] 并发执行多个任务
来源：http://qpy.jinqigfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://llt.cashguo.top

[R37] 把输出赋给变量
来源：http://gia.shanyushiyangkeji.top

files=$(ls -1)
来源：http://bvn.zhaomingkeji.xyz

[R38] 管道串联
来源：http://yyb.ydjk.org.cn

cat a.txt | grep -i error | wc -l
来源：http://eup.gotoacloud.top

[R39] 重定向标准输出与错误
来源：http://ufd.pengpengdd.cyou

cmd > out.log 2>&1
来源：http://voz.bjfxy.top

[R40] 追加写日志
来源：http://yje.havefunace.top

echo "log" >> out.log
来源：http://wcz.mhx1999.top

[R41] 丢弃输出
来源：http://cxs.nanxinkj.top

cmd >/dev/null 2>&1
来源：http://ksl.fzhhl.top

[R42] 输入重定向
来源：http://qoy.snrcjt.cn

wc -l < a.txt
来源：http://jhc.yangfankeji.com

[R43] 按名字查找文件
来源：http://jtp.xylfe.cn

find . -name "*.log" -type f
来源：http://tbj.jqgufenzy.top

[R44] 按修改时间查找
来源：http://pgy.pengpengdd.cyou

find . -mtime -7 -type f
来源：http://lth.guowangkeji.top

[R45] 批量删除
来源：http://yfd.redwolf501.top

find . -name "*.tmp" -delete
来源：http://tje.dashuyun.cn

[R46] 递归替换文件内容
来源：http://eem.uphjek.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fhx.svipenyu.cn

[R47] sed 单行替换
来源：http://fse.jqgufenzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://wst.ehwqpu.com

[R48] awk 取指定列
来源：http://rdr.jinyuanbaomall.cn

awk '{print $1, $3}' a.txt
来源：http://blg.aibaodan.cn

[R49] awk 带条件
来源：http://xyb.meibo888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oxj.daxiang520.top

[R50] awk 求和
来源：http://lpw.jqgufenzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://rjd.dianchejie.cn

[R51] 排序去重取前几
来源：http://lie.yongpay.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mcx.yj20258.top

[R52] 统计行数
来源：http://lsy.guannengcc.top

wc -l a.txt
来源：http://erm.kuanghao11.cn

[R53] 查看文件头与实时尾
来源：http://jxl.sjlbkw.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lia.yongpay.top

[R54] 比较两个文件
来源：http://ogg.gzhubu.top

diff a.txt b.txt
来源：http://syb.shanyushiyangtech.top

[R55] 压缩与解压
来源：http://nun.fengsongda.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hic.bjfxy.top

[R56] 远程拷贝
来源：http://wwz.fzhhl.top

scp file user@host:/path/
来源：http://fcw.hysaishi.cn

[R57] 远程执行命令
来源：http://jbp.yueranfly.top

ssh user@host 'uptime'
来源：http://ukr.xuanzx.com

[R58] 下载文件
来源：http://ckh.zhengqikj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tfo.jinqigufen.top

[R59] 发 POST JSON
来源：http://rdv.yonumen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rho.fengsongda.top

[R60] 只看 HTTP 状态码
来源：http://kjc.shangyingyoupin.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uco.uphjek.com

[R61] 磁盘占用
来源：http://cwx.zdqjudy.top

df -h;  du -sh *
来源：http://vuu.bjfxy.top

[R62] 找最占空间的文件
来源：http://gcb.jiagoushi.top

du -ah . | sort -rh | head -10
来源：http://ljk.hammf.cn

[R63] 内存与进程
来源：http://cfz.zhoulong.xyz

free -h;  ps aux | grep nginx
来源：http://nyc.52xcode.cn

[R64] 结束进程
来源：http://smm.jyoumei.cn

kill -9 $(pgrep -f app.py)
来源：http://wnw.wangdashe.top

[R65] 查看端口占用
来源：http://jzk.yonumen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qoo.gogol.net.cn

[R66] 定时任务
来源：http://bnz.0kj1m.cn

crontab -e;  crontab -l
来源：http://cfw.chenjidiqi.icu

[R67] 生成随机十六进制串
来源：http://iik.zdbjq.cn

openssl rand -hex 16
来源：http://mye.gotoacloud.top

[R68] 计算文件校验值
来源：http://uiu.52xcode.cn

sha256sum a.txt;  md5sum a.txt
来源：http://okd.nanxinkj.top

[R69] 生成随机密码
来源：http://sjl.yfazqb.com

head -c 16 /dev/urandom | base64
来源：http://yqt.jinyuanbaomall.cn

[R70] 时间戳与互转
来源：http://rpa.sufxvd.cn

date +%s;  date -d @1700000000
来源：http://peg.wangdashe.top

[R71] 日期格式化
来源：http://qps.jinqigufen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://gce.pycfn.com

[R72] 等待端口就绪
来源：http://jya.smart0.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://ivq.9152youxi.cn

[R73] 分割大日志
来源：http://npw.ydjk.org.cn

split -l 1000 big.log part_
来源：http://rlo.shzxlz.cn

[R74] 批量重命名
来源：http://rry.316326.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dzv.xuetiantiany.cn

[R75] 导出环境变量
来源：http://ovs.zhoulong.xyz

export PATH="$HOME/bin:$PATH"
来源：http://zho.yonumen.top

[R76] 使用临时文件
来源：http://pch.daria6918.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jpb.yvedp.cn

[R77] 读取用户输入
来源：http://ocn.shanyushiyangkeji.top

read -rp "请输入: " ans
来源：http://din.hnqzz.top

[R78] 交互式菜单
来源：http://bkj.ehwqpu.com

select opt in a b c; do echo "$opt"; break; done
来源：http://uqu.tian-w.cn

[R79] 解析命令行选项
来源：http://cqt.jqgfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xom.yfazqb.com

[R80] 查看脚本执行耗时
来源：http://sys.dianchejie.cn

time ./run.sh
来源：http://bwl.nwbrower.top

================================================================================
来源：http://qxu.xinyue.icu

S. C / C++ 专题
来源：http://lzm.zhoulong.xyz

================================================================================
来源：http://bmk.aibaodan.cn

[S01] C：Hello World
来源：http://efu.zhoulong.xyz

#include <stdio.h>
来源：http://lup.fengsongda.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://pwx.zhaomingkeji.xyz

[S02] C：变量与格式化输出
来源：http://vgk.svipenyu.cn

int a = 10; printf("%d\n", a);
来源：http://vef.yj202588.top

[S03] C：读入整数
来源：http://ljm.cucudq.cn

int x; scanf("%d", &x);
来源：http://ckp.hnxiangtu.top

[S04] C：字符串复制
来源：http://bjj.tanke756.top

char dst[32]; strcpy(dst, "hi");
来源：http://sky.svipenyu.cn

[S05] C：字符串长度
来源：http://vnc.shzxlz.cn

strlen(s)
来源：http://hxl.aizwys.cn

[S06] C：字符串比较
来源：http://igk.sxryk.cn

strcmp(a, b) == 0
来源：http://chi.fanxiaobao.xyz

[S07] C：数组遍历求和
来源：http://xmm.sweek.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hrc.ctjpmb.com

[S08] C：动态内存分配与释放
来源：http://gfs.zhongyouzk.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sfb.bbcook.cn

[S09] C：结构体定义与初始化
来源：http://nao.cheryme.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://aek.quarkkingdee.top

[S10] C：指针与解引用
来源：http://mgq.tarul.cn

int *p = &a;  *p = 5;
来源：http://bvq.ctjpmb.com

[S11] C：逐行读文件
来源：http://laz.nanxuanxn.top

FILE *f = fopen("a.txt", "r");
来源：http://cxm.smart0.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://yck.ppjwa.cn

fclose(f);
来源：http://bwb.hammf.cn

[S12] C：写文件
来源：http://mte.jiagoushi.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uex.jiagoushi.top

[S13] C：宏定义
来源：http://lsx.zhixingplan.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kmi.ybcxt.top

[S14] C：枚举
来源：http://aby.zdqjudy.top

enum Color { RED, GREEN, BLUE };
来源：http://eef.nwbrower.top

[S15] C：类型转换
来源：http://ehw.ywan-chungtsiang.top

(double) a / b
来源：http://nyo.shangyingyoupin.top

[S16] C：位操作置位
来源：http://mcv.mhx1999.top

x |= (1 << 3);
来源：http://pyy.9152youxi.cn

[S17] C：安全拼接字符串
来源：http://dcg.yanxiufei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pgt.yvedp.cn

[S18] C：命令行参数
来源：http://sug.yangfankeji.com

int main(int argc, char **argv)
来源：http://kfq.meibo888.top

[S19] C：快速排序
来源：http://hje.sxryk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kdw.xuanzx.com

[S20] C：二分查找
来源：http://sex.shanyushiyangtech.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qws.yuanzhike.top

[S21] C：字符类别判断
来源：http://wvp.xinyue.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ofd.nanxinkj.top

[S22] C：字符串转数字
来源：http://ewg.cheryme.top

atoi("42");  strtod("3.14", NULL);
来源：http://twn.quarkkingdee.top

[S23] C：随机数
来源：http://cxk.cucudq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yrf.dianchejie.cn

[S24] C：获取本地时间
来源：http://nhe.cashguo.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hbh.kuanghao11.cn

[S25] C：内存拷贝
来源：http://qhx.ehwqpu.com

memcpy(dst, src, n);
来源：http://mzu.fanxiaobao.xyz

[S26] C：内存清零
来源：http://swm.hesvh.cn

memset(a, 0, sizeof a);
来源：http://gjx.kuanghao11.cn

[S27] C：定义常量
来源：http://ilf.aizwys.cn

const double PI = 3.14159;
来源：http://ebj.fehbvm.com

[S28] C：静态变量
来源：http://cxf.jqgfzy.top

static int counter = 0;
来源：http://zbv.xingfuxueyuan.xyz

[S29] C：变参函数
来源：http://hcb.sufxvd.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cre.sjlbkw.cn

[S30] C：头文件保护
来源：http://jjw.shanyushiyangtech.top

#ifndef X_H
来源：http://ayp.cdnleiting.top

#define X_H
来源：http://elc.shanyushiyangkeji.top

#endif
来源：http://ftu.jlsjyb.cn

[S31] C++：Hello World
来源：http://ppt.hammf.cn

#include <iostream>
来源：http://fwi.zdbjq.cn

int main() { std::cout << "Hello\n"; }
来源：http://kuf.0kj1m.cn

[S32] C++：字符串
来源：http://cjo.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://osx.hnqzz.top

[S33] C++：vector 增删
来源：http://sdi.wangshuangyany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dxs.ydjk.org.cn

[S34] C++：遍历 vector
来源：http://txc.gaohongyu789.top

for (auto &x : v) { std::cout << x; }
来源：http://chr.hnxiangtu.top

[S35] C++：map
来源：http://pqw.svipenyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vlk.hysaishi.cn

[S36] C++：unordered_map
来源：http://wfm.gzhubu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ngt.xziqi.cn

[S37] C++：set
来源：http://zom.vehdjk.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://aal.uphjek.com

[S38] C++：排序
来源：http://avl.sufxvd.cn

std::sort(v.begin(), v.end());
来源：http://ofn.ivvv.top

[S39] C++：自定义比较器排序
来源：http://flh.havefunace.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://obo.fengsongda.top

[S40] C++：查找元素
来源：http://caz.snrcjt.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hqd.52xcode.cn

[S41] C++：类与构造函数
来源：http://rxc.316326.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dlp.jqgfzy.top

[S42] C++：继承与虚函数
来源：http://noz.fengsongda.top

class B : public Base { public: void f() override {} };
来源：http://rbq.gaohongyu789.top

[S43] C++：智能指针
来源：http://lyn.havefunace.top

auto p = std::make_unique<int>(5);
来源：http://jtz.xylfe.cn

[S44] C++：引用传参
来源：http://zov.zhixingplan.top

void inc(int &x) { ++x; }
来源：http://ewt.jyoumei.cn

[S45] C++：lambda
来源：http://qsf.jqgufenzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://jap.jianghu66.top

[S46] C++：函数模板
来源：http://qob.yvedp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zab.shangyingyoupin.top

[S47] C++：结构化绑定遍历
来源：http://unu.zdbjq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lcm.snrcjt.cn

[S48] C++：逐行读文件
来源：http://cva.birdmap.top

std::ifstream in("a.txt");  std::string line;
来源：http://ggh.shanyushiyangtech.top

while (std::getline(in, line)) { }
来源：http://yww.ydjk.org.cn

[S49] C++：写文件
来源：http://wmj.chenjidiqi.icu

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lwe.tianlin.xyz

[S50] C++：格式化数字
来源：http://vnd.yanxiufei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hwi.hesvh.cn

[S51] C++：显式类型转换
来源：http://nyj.sweek.top

static_cast<double>(a) / b
来源：http://amq.sysykeji.top

[S52] C++：const 与 noexcept
来源：http://zxp.yueranfly.top

int size() const noexcept { return n_; }
来源：http://zbf.mhx1999.top

[S53] C++：移动语义
来源：http://nig.nwbrower.top

std::vector<int> w = std::move(v);
来源：http://woy.yj202588.top

[S54] C++：异常处理
来源：http://aaq.nwbrower.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kyd.birdmap.top

[S55] C++：结构化绑定
来源：http://hrx.cucudq.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tii.guannengcc.top

[S56] C++：optional
来源：http://khw.yj20258.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uia.xuetiantiany.cn

[S57] C++：编译期常量
来源：http://prs.hfpthk.cn

constexpr int N = 10;
来源：http://cuy.fengsongda.top

[S58] C++：命名空间
来源：http://yfb.yanxiufei.cn

namespace ns { int f() { return 1; } }
来源：http://kni.ctjpmb.com

[S59] C++：静态断言
来源：http://tjk.fanxiaobao.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pdt.chenjidiqi.icu

[S60] C++：遍历并删除元素
来源：http://owc.snrcjt.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hhf.jiagoushi.top

================================================================================
来源：http://oik.wangshuangyany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tga.dashuyun.cn

================================================================================
来源：http://mnd.gogol.net.cn

[T01] Kotlin：Hello World
来源：http://kjf.jiagoushi.top

println("Hello")
来源：http://flj.mhx1999.top

[T02] Kotlin：变量
来源：http://bpn.ywan-chungtsiang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ltj.gzhubu.top

[T03] Kotlin：字符串模板
来源：http://fzj.yongpay.top

"值: $b"
来源：http://hyr.jinqigfzy.top

[T04] Kotlin：空安全
来源：http://kgs.zycfv.cn

val n: String? = null;  n?.length
来源：http://tpr.wangdashe.top

[T05] Kotlin：when 表达式
来源：http://bwv.jiagoushi.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xet.0kj1m.cn

[T06] Kotlin：集合映射
来源：http://lge.jiagoushi.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rwn.52xcode.cn

[T07] Kotlin：集合过滤
来源：http://hkm.smart0.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://foo.hongshengwenyu.top

[T08] Kotlin：数据类
来源：http://ywl.xuetiantiany.cn

data class User(val name: String, val age: Int)
来源：http://fia.gzhubu.top

[T09] Kotlin：扩展函数
来源：http://mdo.tarul.cn

fun String.exclaim() = this + "!"
来源：http://djr.fanxiaobao.xyz

[T10] Kotlin：默认参数
来源：http://lpd.zhijiandao.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://btz.hnqzz.top

[T11] Kotlin：协程
来源：http://dqe.yongpay.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qlh.52xcode.cn

[T12] Kotlin：解构声明
来源：http://jdz.vehdjk.com

val (a, b) = Pair(1, 2)
来源：http://pea.vqdsnc.cn

[T13] Kotlin：只读 Map
来源：http://glm.jinqigufen.top

val m = mapOf("a" to 1)
来源：http://kfk.jqgfzy.top

[T14] Kotlin：循环
来源：http://bxs.bbcook.cn

for (i in 1..10) println(i)
来源：http://xuy.hcnkem.com

[T15] Kotlin：接口
来源：http://oku.yangfankeji.com

interface Shape { fun area(): Double }
来源：http://xqb.hammf.cn

[T16] Swift：Hello World
来源：http://gjx.ehwqpu.com

print("Hello")
来源：http://vsy.zhijiandao.cn

[T17] Swift：变量与常量
来源：http://obi.zhixingplan.top

var a = 1;  let b = 2
来源：http://wbh.xuanzx.com

[T18] Swift：字符串插值
来源：http://gzx.birdmap.top

"值: \(b)"
来源：http://mrf.birdmap.top


<!-- 参考信息 -->