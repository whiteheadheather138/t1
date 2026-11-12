代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://gyk.pengpengdd.cyou

[R14] C 风格 for
来源：http://vrj.hnxiangtu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dip.xinyue.icu

[R15] while 逐行读文件
来源：http://aln.daria6918.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dcg.shuidangran.top

[R16] until 等待条件
来源：http://bah.nanxinkj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cvi.ivvv.top

[R17] 数组定义与取值
来源：http://xby.svipenyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sdp.hywenlv.cn

[R18] 遍历数组
来源：http://nnb.zdbjq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://waa.zhengqikj.top

[R19] 数组长度
来源：http://rwa.gaohongyu789.top

echo "${#arr[@]}"
来源：http://pgg.yfazqb.com

[R20] 关联数组（字典）
来源：http://lga.daxiang520.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vrw.fehbvm.com

[R21] 字符串长度
来源：http://yxd.yangfankeji.com

echo "${#s}"
来源：http://knr.yuanzhike.top

[R22] 截取子串
来源：http://xmz.aibaodan.cn

echo "${s:0:5}"
来源：http://uwc.zhoulong.xyz

[R23] 字符串替换
来源：http://vzc.jinghuilouyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ivs.bjfxy.top

[R24] 大小写转换
来源：http://dvx.yongpay.top

echo "${s^^}"; echo "${s,,}"
来源：http://xqy.sufxvd.cn

[R25] 去后缀 / 去前缀
来源：http://mtc.cashguo.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zbi.dashuyun.cn

[R26] 命令替换
来源：http://tzz.zhaomingkeji.xyz

now=$(date +%F); echo "$now"
来源：http://omb.sysykeji.top

[R27] 算术展开
来源：http://lgc.xuetiantiany.cn

echo $((1 + 2 * 3))
来源：http://bjv.jlsjyb.cn

[R28] 浮点运算
来源：http://adt.birdmap.top

echo "scale=2; 10/3" | bc
来源：http://kur.hfpthk.cn

[R29] 定义函数
来源：http://dwr.andypj.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mzt.zhixingplan.top

[R30] 函数返回状态码
来源：http://zfg.kuanghao11.cn

f() { return 0; }; f || echo "失败了"
来源：http://kov.andypj.xyz

[R31] 局部变量
来源：http://nib.jianghu66.top

f() { local x=1; echo "$x"; }
来源：http://ngo.havefunace.top

[R32] 参数个数校验
来源：http://jyo.snrcjt.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vvl.nwbrower.top

[R33] 捕获错误并提示行号
来源：http://zmz.andypj.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cuj.yvedp.cn

[R34] 退出时清理
来源：http://hwp.hnqzz.top

trap 'rm -f "$tmp"' EXIT
来源：http://nbn.zhiwuduotai.top

[R35] 后台执行并等待
来源：http://clv.gzhubu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://txm.fengsongda.top

[R36] 并发执行多个任务
来源：http://uwi.cucudq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nzl.hfpthk.cn

[R37] 把输出赋给变量
来源：http://rwm.sjlbkw.cn

files=$(ls -1)
来源：http://jcl.yonumen.top

[R38] 管道串联
来源：http://lih.ydzc1.top

cat a.txt | grep -i error | wc -l
来源：http://kir.hywenlv.cn

[R39] 重定向标准输出与错误
来源：http://tgg.gotoacloud.top

cmd > out.log 2>&1
来源：http://vbh.yj20258888.top

[R40] 追加写日志
来源：http://bvb.sysykeji.top

echo "log" >> out.log
来源：http://fhk.redwolf501.top

[R41] 丢弃输出
来源：http://iwt.9152youxi.cn

cmd >/dev/null 2>&1
来源：http://yfl.9152youxi.cn

[R42] 输入重定向
来源：http://esh.guannengcc.top

wc -l < a.txt
来源：http://zaj.shanyushiyangkeji.top

[R43] 按名字查找文件
来源：http://kfs.ywan-chungtsiang.top

find . -name "*.log" -type f
来源：http://qcq.xuanzx.com

[R44] 按修改时间查找
来源：http://cow.0kj1m.cn

find . -mtime -7 -type f
来源：http://nqs.chenlongwang.top

[R45] 批量删除
来源：http://ffo.shangyingyoupin.top

find . -name "*.tmp" -delete
来源：http://pgx.hywenlv.cn

[R46] 递归替换文件内容
来源：http://sht.ctjpmb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cra.jyoumei.cn

[R47] sed 单行替换
来源：http://znn.chenlongwang.top

sed -i 's/foo/bar/g' a.txt
来源：http://nqy.svipenyu.cn

[R48] awk 取指定列
来源：http://nxf.sysykeji.top

awk '{print $1, $3}' a.txt
来源：http://tin.9152youxi.cn

[R49] awk 带条件
来源：http://dfe.xuanzx.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vic.sufxvd.cn

[R50] awk 求和
来源：http://sho.jinqigfzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://ztd.ivvv.top

[R51] 排序去重取前几
来源：http://hpm.jiagoushi.top

sort a.txt | uniq -c | sort -rn | head
来源：http://lhm.cdnleiting.top

[R52] 统计行数
来源：http://dan.nanxuanxn.top

wc -l a.txt
来源：http://cwv.gotoacloud.top

[R53] 查看文件头与实时尾
来源：http://eal.ydzc1.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ukj.aizwys.cn

[R54] 比较两个文件
来源：http://ndf.nanxuanxn.top

diff a.txt b.txt
来源：http://xkv.ydzc1.top

[R55] 压缩与解压
来源：http://xvw.sysykeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fqh.gzhubu.top

[R56] 远程拷贝
来源：http://jcl.bjfxy.top

scp file user@host:/path/
来源：http://xnj.haohaochexian.top

[R57] 远程执行命令
来源：http://wgz.yvedp.cn

ssh user@host 'uptime'
来源：http://phm.sweek.top

[R58] 下载文件
来源：http://qjv.316326.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jqm.zhaomingkeji.xyz

[R59] 发 POST JSON
来源：http://ltz.nanxinkj.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pgv.gaohongyu789.top

[R60] 只看 HTTP 状态码
来源：http://xpp.ehwqpu.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cjb.yfazqb.com

[R61] 磁盘占用
来源：http://dus.xinyue.icu

df -h;  du -sh *
来源：http://wqo.fanxiaobao.xyz

[R62] 找最占空间的文件
来源：http://vip.gogol.net.cn

du -ah . | sort -rh | head -10
来源：http://hjg.bjfxy.top

[R63] 内存与进程
来源：http://oyd.nanxinkj.top

free -h;  ps aux | grep nginx
来源：http://krt.wangdashe.top

[R64] 结束进程
来源：http://jyb.zdqjudy.top

kill -9 $(pgrep -f app.py)
来源：http://hls.yongpay.top

[R65] 查看端口占用
来源：http://axt.zhaomingkeji.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ojq.yj20258888.top

[R66] 定时任务
来源：http://knr.xylfe.cn

crontab -e;  crontab -l
来源：http://npf.hesvh.cn

[R67] 生成随机十六进制串
来源：http://ljf.quarkkingdee.top

openssl rand -hex 16
来源：http://tdv.zdbjq.cn

[R68] 计算文件校验值
来源：http://zci.haohaochexian.top

sha256sum a.txt;  md5sum a.txt
来源：http://jus.jianghu66.top

[R69] 生成随机密码
来源：http://riq.chenzaomai.com

head -c 16 /dev/urandom | base64
来源：http://ssr.chenzaomai.com

[R70] 时间戳与互转
来源：http://igk.jqgfzy.top

date +%s;  date -d @1700000000
来源：http://buk.chenlongwang.top

[R71] 日期格式化
来源：http://iqx.ywan-chungtsiang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://hnl.andypj.xyz

[R72] 等待端口就绪
来源：http://rnq.52xcode.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lca.jianghu66.top

[R73] 分割大日志
来源：http://jbv.feifeiyinyue.top

split -l 1000 big.log part_
来源：http://mxt.hammf.cn

[R74] 批量重命名
来源：http://lmo.chenlongwang.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://txa.svipenyu.cn

[R75] 导出环境变量
来源：http://yms.mhx1999.top

export PATH="$HOME/bin:$PATH"
来源：http://nvx.smart0.xyz

[R76] 使用临时文件
来源：http://cdq.xingfuxueyuan.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jfb.sysykeji.top

[R77] 读取用户输入
来源：http://iij.vehdjk.com

read -rp "请输入: " ans
来源：http://jni.52xcode.cn

[R78] 交互式菜单
来源：http://tmz.shanyushiyangkeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://fad.jinyuanbaomall.cn

[R79] 解析命令行选项
来源：http://qko.fzhhl.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://etd.nanxinkj.top

[R80] 查看脚本执行耗时
来源：http://niu.iojbl.cn

time ./run.sh
来源：http://drs.zhaomingkeji.xyz

================================================================================
来源：http://bar.hnxiangtu.top

S. C / C++ 专题
来源：http://tjw.cdnleiting.top

================================================================================
来源：http://cvp.yanxiufei.cn

[S01] C：Hello World
来源：http://tvv.bjfxy.top

#include <stdio.h>
来源：http://hyt.cdnleiting.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://osu.yuxming.cn

[S02] C：变量与格式化输出
来源：http://zby.yueranfly.top

int a = 10; printf("%d\n", a);
来源：http://azr.xylfe.cn

[S03] C：读入整数
来源：http://kjk.svipenyu.cn

int x; scanf("%d", &x);
来源：http://bdz.dashuyun.cn

[S04] C：字符串复制
来源：http://wpn.bjfxy.top

char dst[32]; strcpy(dst, "hi");
来源：http://dac.aibaodan.cn

[S05] C：字符串长度
来源：http://gsk.ctjpmb.com

strlen(s)
来源：http://xoz.zhiwuduotai.top

[S06] C：字符串比较
来源：http://fdc.zhongyouzk.top

strcmp(a, b) == 0
来源：http://xwd.xuetiantiany.cn

[S07] C：数组遍历求和
来源：http://jgt.fktsv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://glu.yj20258.top

[S08] C：动态内存分配与释放
来源：http://rns.yj202588.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wen.yfazqb.com

[S09] C：结构体定义与初始化
来源：http://ssl.smart0.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zzz.jinyuanbaomall.cn

[S10] C：指针与解引用
来源：http://euh.nanxinkj.top

int *p = &a;  *p = 5;
来源：http://wym.ppjwa.cn

[S11] C：逐行读文件
来源：http://avu.hesvh.cn

FILE *f = fopen("a.txt", "r");
来源：http://fwa.redwolf501.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://mpk.xinyue.icu

fclose(f);
来源：http://rea.birdmap.top

[S12] C：写文件
来源：http://vdx.hywenlv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fau.haohaochexian.top

[S13] C：宏定义
来源：http://ify.uphjek.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://odx.zdqjudy.top

[S14] C：枚举
来源：http://gyd.yfazqb.com

enum Color { RED, GREEN, BLUE };
来源：http://zux.hongshengwenyu.top

[S15] C：类型转换
来源：http://ghr.hcnkem.com

(double) a / b
来源：http://mmc.shanyushiyangtech.top

[S16] C：位操作置位
来源：http://ngj.cdnleiting.top

x |= (1 << 3);
来源：http://pcl.zhijiandao.cn

[S17] C：安全拼接字符串
来源：http://ubh.smart0.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uis.vqdsnc.cn

[S18] C：命令行参数
来源：http://aaa.hnxiangtu.top

int main(int argc, char **argv)
来源：http://hdp.cdnleiting.top

[S19] C：快速排序
来源：http://pvc.pycfn.com

qsort(a, n, sizeof(int), cmp);
来源：http://utr.tianlin.xyz

[S20] C：二分查找
来源：http://fud.yfazqb.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://orw.hammf.cn

[S21] C：字符类别判断
来源：http://uvw.tarul.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wyx.zhoulong.xyz

[S22] C：字符串转数字
来源：http://cwu.guannengcc.top

atoi("42");  strtod("3.14", NULL);
来源：http://xva.hammf.cn

[S23] C：随机数
来源：http://oyb.xinyue.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://izg.xylfe.cn

[S24] C：获取本地时间
来源：http://hpo.dashuyun.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eyg.jqgufenzy.top

[S25] C：内存拷贝
来源：http://xlo.shanyushiyangkeji.top

memcpy(dst, src, n);
来源：http://vdg.yuanzhike.top

[S26] C：内存清零
来源：http://zbi.yuxming.cn

memset(a, 0, sizeof a);
来源：http://wxa.c1oappe.top

[S27] C：定义常量
来源：http://uvv.bjfxy.top

const double PI = 3.14159;
来源：http://rez.zhoulong.xyz

[S28] C：静态变量
来源：http://jnd.uphjek.com

static int counter = 0;
来源：http://wsh.cheryme.top

[S29] C：变参函数
来源：http://zyb.ppjwa.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dzi.gzhubu.top

[S30] C：头文件保护
来源：http://tga.sysykeji.top

#ifndef X_H
来源：http://wkj.jlsjyb.cn

#define X_H
来源：http://nau.hfpthk.cn

#endif
来源：http://liy.fktsv.cn

[S31] C++：Hello World
来源：http://pxu.birdmap.top

#include <iostream>
来源：http://zms.chenjidiqi.icu

int main() { std::cout << "Hello\n"; }
来源：http://hwz.kuanghao11.cn

[S32] C++：字符串
来源：http://tqk.shzxlz.cn

std::string s = "hi";  s += "!";
来源：http://zgf.iojbl.cn

[S33] C++：vector 增删
来源：http://hbx.hnqzz.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lhj.hnxiangtu.top

[S34] C++：遍历 vector
来源：http://btp.snrcjt.cn

for (auto &x : v) { std::cout << x; }
来源：http://dtf.jqgfzy.top

[S35] C++：map
来源：http://dbx.ctjpmb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dov.ybcxt.top

[S36] C++：unordered_map
来源：http://kqp.fengsongda.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ixs.pengpengdd.cyou

[S37] C++：set
来源：http://xwj.c1oappe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iaf.cheryme.top

[S38] C++：排序
来源：http://sag.52xcode.cn

std::sort(v.begin(), v.end());
来源：http://vrm.kuanghao11.cn

[S39] C++：自定义比较器排序
来源：http://ykw.daria6918.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lxg.sxryk.cn

[S40] C++：查找元素
来源：http://qym.chenlongwang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://quz.hnqzz.top

[S41] C++：类与构造函数
来源：http://ybu.yonumen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fog.jinghuilouyu.cn

[S42] C++：继承与虚函数
来源：http://bgd.zdbjq.cn

class B : public Base { public: void f() override {} };
来源：http://haa.ydzc1.top

[S43] C++：智能指针
来源：http://wis.gotoacloud.top

auto p = std::make_unique<int>(5);
来源：http://kmh.yj20258888.top

[S44] C++：引用传参
来源：http://tto.ybcxt.top

void inc(int &x) { ++x; }
来源：http://aqw.haohaochexian.top

[S45] C++：lambda
来源：http://myx.zhoulong.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://gfb.zhixingplan.top

[S46] C++：函数模板
来源：http://hvd.tanke756.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://igi.nanxuanxn.top

[S47] C++：结构化绑定遍历
来源：http://hpu.sweek.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cmc.yueranfly.top

[S48] C++：逐行读文件
来源：http://dkm.zhoulong.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://npi.shuidangran.top

while (std::getline(in, line)) { }
来源：http://xfg.gzhubu.top

[S49] C++：写文件
来源：http://pdl.bbcook.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lie.guowangkeji.top

[S50] C++：格式化数字
来源：http://ugu.kuanghao11.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://odv.tarul.cn

[S51] C++：显式类型转换
来源：http://aeq.shzxlz.cn

static_cast<double>(a) / b
来源：http://qfj.fengsongda.top

[S52] C++：const 与 noexcept
来源：http://pbq.chenzaomai.com

int size() const noexcept { return n_; }
来源：http://vns.iojbl.cn

[S53] C++：移动语义
来源：http://gom.nwbrower.top

std::vector<int> w = std::move(v);
来源：http://btr.wangshuangyany.cn

[S54] C++：异常处理
来源：http://zcj.fengsongda.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gbw.birdmap.top

[S55] C++：结构化绑定
来源：http://mpg.tianlin.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://jkm.yj20258888.top

[S56] C++：optional
来源：http://wjl.cashguo.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eve.hfpthk.cn

[S57] C++：编译期常量
来源：http://nws.yj20258.top

constexpr int N = 10;
来源：http://jar.zhixingplan.top

[S58] C++：命名空间
来源：http://wos.guannengcc.top

namespace ns { int f() { return 1; } }
来源：http://pzt.cashguo.top

[S59] C++：静态断言
来源：http://gdq.zhoulong.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ojw.nwbrower.top

[S60] C++：遍历并删除元素
来源：http://caf.ydzc1.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yie.aizwys.cn

================================================================================
来源：http://chn.bjfxy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://esl.snrcjt.cn

================================================================================
来源：http://ttc.sufxvd.cn

[T01] Kotlin：Hello World
来源：http://sez.xingfuxueyuan.xyz

println("Hello")
来源：http://rdw.yj20258888.top

[T02] Kotlin：变量
来源：http://rsy.ivvv.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wcn.cashguo.top

[T03] Kotlin：字符串模板
来源：http://gar.bbcook.cn

"值: $b"
来源：http://tib.ydzc1.top

[T04] Kotlin：空安全
来源：http://nom.haohaochexian.top

val n: String? = null;  n?.length
来源：http://zre.jinyuanbaomall.cn

[T05] Kotlin：when 表达式
来源：http://ejh.hammf.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wsd.ivvv.top

[T06] Kotlin：集合映射
来源：http://ujl.yongpay.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qaq.aibaodan.cn

[T07] Kotlin：集合过滤
来源：http://art.nwbrower.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://lic.yj20258888.top

[T08] Kotlin：数据类
来源：http://bin.xylfe.cn

data class User(val name: String, val age: Int)
来源：http://qvb.zhiwuduotai.top

[T09] Kotlin：扩展函数
来源：http://ntp.zhiwuduotai.top

fun String.exclaim() = this + "!"
来源：http://yno.bbcook.cn

[T10] Kotlin：默认参数
来源：http://cra.ywan-chungtsiang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ior.cucudq.cn

[T11] Kotlin：协程
来源：http://bmx.redwolf501.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://tna.nanxinkj.top

[T12] Kotlin：解构声明
来源：http://gbi.nwbrower.top

val (a, b) = Pair(1, 2)
来源：http://kct.birdmap.top

[T13] Kotlin：只读 Map
来源：http://gmg.jiagoushi.top

val m = mapOf("a" to 1)
来源：http://kbo.jianghu66.top

[T14] Kotlin：循环
来源：http://cuo.zhiwuduotai.top

for (i in 1..10) println(i)
来源：http://zcn.mhx1999.top

[T15] Kotlin：接口
来源：http://zoh.quarkkingdee.top

interface Shape { fun area(): Double }
来源：http://vup.yueranfly.top

[T16] Swift：Hello World
来源：http://koa.guowangkeji.top

print("Hello")
来源：http://zwe.yuxming.cn


<!-- 参考信息 -->