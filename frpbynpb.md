代发 wailian999

readonly PI=3.14
来源：http://ntd.tarul.cn

[R04] 位置参数
来源：http://goe.jinyuanbaomall.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cxw.gogol.net.cn

[R05] 参数默认值
来源：http://tkw.wangshuangyany.cn

name="${1:-default}"
来源：http://eaa.xingfuxueyuan.xyz

[R06] 判断命令是否存在
来源：http://kmn.bjfxy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oad.dashuyun.cn

[R07] if 判断文件
来源：http://nsq.snrcjt.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xtn.yfazqb.com

[R08] 数值比较
来源：http://jfj.gotoacloud.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vly.hesvh.cn

[R09] 字符串比较
来源：http://xrj.hesvh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://eqx.yj20258888.top

[R10] 正则匹配
来源：http://rvn.kuanghao11.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sol.xinyue.icu

[R11] case 多分支
来源：http://dng.guannengcc.top

case "$1" in
来源：http://gam.zhoulong.xyz

start) echo "启动" ;;
来源：http://bet.xylfe.cn

stop)  echo "停止" ;;
来源：http://hrj.xylfe.cn

*)     echo "未知命令" ;;
来源：http://rbc.nanxinkj.top

esac
来源：http://bvo.aizwys.cn

[R12] for 遍历文件
来源：http://aia.yanxiufei.cn

for f in *.txt; do echo "$f"; done
来源：http://hsz.9152youxi.cn

[R13] for 计数循环
来源：http://bmj.nanxuanxn.top

for i in {1..10}; do echo "$i"; done
来源：http://hyq.fengsongda.top

[R14] C 风格 for
来源：http://the.cdnleiting.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ifi.cheryme.top

[R15] while 逐行读文件
来源：http://ijm.daxiang520.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uvb.birdmap.top

[R16] until 等待条件
来源：http://ukh.daxiang520.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://miv.jqgufenzy.top

[R17] 数组定义与取值
来源：http://hdm.aibaodan.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gur.quarkkingdee.top

[R18] 遍历数组
来源：http://xad.birdmap.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gjz.zhijiandao.cn

[R19] 数组长度
来源：http://fug.birdmap.top

echo "${#arr[@]}"
来源：http://ihl.hnxiangtu.top

[R20] 关联数组（字典）
来源：http://zkm.sxryk.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kzp.dianchejie.cn

[R21] 字符串长度
来源：http://biv.chenjidiqi.icu

echo "${#s}"
来源：http://dfr.tianlin.xyz

[R22] 截取子串
来源：http://jqg.wangshuangyany.cn

echo "${s:0:5}"
来源：http://txi.gotoacloud.top

[R23] 字符串替换
来源：http://gzz.sweek.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hug.hcnkem.com

[R24] 大小写转换
来源：http://rpp.ppjwa.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mgn.jianghu66.top

[R25] 去后缀 / 去前缀
来源：http://mle.shuidangran.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://aft.bbcook.cn

[R26] 命令替换
来源：http://igh.jinyuanbaomall.cn

now=$(date +%F); echo "$now"
来源：http://bld.hammf.cn

[R27] 算术展开
来源：http://bre.zhoulong.xyz

echo $((1 + 2 * 3))
来源：http://aaj.zdqjudy.top

[R28] 浮点运算
来源：http://qca.ivvv.top

echo "scale=2; 10/3" | bc
来源：http://zjk.hywenlv.cn

[R29] 定义函数
来源：http://qvt.nwbrower.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uax.dianchejie.cn

[R30] 函数返回状态码
来源：http://xaq.yfazqb.com

f() { return 0; }; f || echo "失败了"
来源：http://egc.ywan-chungtsiang.top

[R31] 局部变量
来源：http://sge.nanxuanxn.top

f() { local x=1; echo "$x"; }
来源：http://mpe.yanxiufei.cn

[R32] 参数个数校验
来源：http://ubq.cqqwz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qza.jlsjyb.cn

[R33] 捕获错误并提示行号
来源：http://koh.hywenlv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ssg.cashguo.top

[R34] 退出时清理
来源：http://kdh.fktsv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zdd.smart0.xyz

[R35] 后台执行并等待
来源：http://vyc.chenzaomai.com

sleep 5 & pid=$!; wait "$pid"
来源：http://dje.zycfv.cn

[R36] 并发执行多个任务
来源：http://ltf.wangshuangyany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vuy.ydzc1.top

[R37] 把输出赋给变量
来源：http://saq.cqqwz.cn

files=$(ls -1)
来源：http://uwl.jianghu66.top

[R38] 管道串联
来源：http://lrk.pengpengdd.cyou

cat a.txt | grep -i error | wc -l
来源：http://fpz.nanxinkj.top

[R39] 重定向标准输出与错误
来源：http://glp.shangyingyoupin.top

cmd > out.log 2>&1
来源：http://flb.tianlin.xyz

[R40] 追加写日志
来源：http://ywq.dashuyun.cn

echo "log" >> out.log
来源：http://tiv.fktsv.cn

[R41] 丢弃输出
来源：http://dnl.fanxiaobao.xyz

cmd >/dev/null 2>&1
来源：http://vxx.sysykeji.top

[R42] 输入重定向
来源：http://ucz.zdqjudy.top

wc -l < a.txt
来源：http://hso.hfpthk.cn

[R43] 按名字查找文件
来源：http://bbk.zdqjudy.top

find . -name "*.log" -type f
来源：http://bme.fzhhl.top

[R44] 按修改时间查找
来源：http://vmx.andypj.xyz

find . -mtime -7 -type f
来源：http://aih.zhiwuduotai.top

[R45] 批量删除
来源：http://lso.fktsv.cn

find . -name "*.tmp" -delete
来源：http://nwh.vehdjk.com

[R46] 递归替换文件内容
来源：http://vjl.hnxiangtu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nap.feifeiyinyue.top

[R47] sed 单行替换
来源：http://lkq.daria6918.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yuj.jiagoushi.top

[R48] awk 取指定列
来源：http://tij.xziqi.cn

awk '{print $1, $3}' a.txt
来源：http://yte.havefunace.top

[R49] awk 带条件
来源：http://iza.wangshuangyany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vzz.quarkkingdee.top

[R50] awk 求和
来源：http://nkz.zhongyouzk.top

awk '{s += $2} END {print s}' a.txt
来源：http://kdf.vehdjk.com

[R51] 排序去重取前几
来源：http://ixp.xylfe.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zhk.wangdashe.top

[R52] 统计行数
来源：http://rle.ybcxt.top

wc -l a.txt
来源：http://ljh.svipenyu.cn

[R53] 查看文件头与实时尾
来源：http://top.zhaomingkeji.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pkb.quarkkingdee.top

[R54] 比较两个文件
来源：http://cjt.ybcxt.top

diff a.txt b.txt
来源：http://bvd.sxryk.cn

[R55] 压缩与解压
来源：http://dby.xuetiantiany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xgs.zdqjudy.top

[R56] 远程拷贝
来源：http://zgc.fehbvm.com

scp file user@host:/path/
来源：http://pii.tanke756.top

[R57] 远程执行命令
来源：http://ywk.vqdsnc.cn

ssh user@host 'uptime'
来源：http://xvo.jqgufenzy.top

[R58] 下载文件
来源：http://gxj.chenlongwang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nvf.bjfxy.top

[R59] 发 POST JSON
来源：http://ffm.yj20258888.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yms.vehdjk.com

[R60] 只看 HTTP 状态码
来源：http://chw.shanyushiyangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ndu.pengpengdd.cyou

[R61] 磁盘占用
来源：http://iws.ppjwa.cn

df -h;  du -sh *
来源：http://ttc.ctjpmb.com

[R62] 找最占空间的文件
来源：http://aqr.ybcxt.top

du -ah . | sort -rh | head -10
来源：http://gtc.zhengqikj.top

[R63] 内存与进程
来源：http://wrx.zycfv.cn

free -h;  ps aux | grep nginx
来源：http://rbb.fehbvm.com

[R64] 结束进程
来源：http://jbj.yfazqb.com

kill -9 $(pgrep -f app.py)
来源：http://abr.fehbvm.com

[R65] 查看端口占用
来源：http://mly.aizwys.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cdy.gzhubu.top

[R66] 定时任务
来源：http://zuy.yj20258888.top

crontab -e;  crontab -l
来源：http://nnx.quarkkingdee.top

[R67] 生成随机十六进制串
来源：http://toh.yonumen.top

openssl rand -hex 16
来源：http://ags.yfazqb.com

[R68] 计算文件校验值
来源：http://orn.wangshuangyany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pha.hammf.cn

[R69] 生成随机密码
来源：http://jji.zdbjq.cn

head -c 16 /dev/urandom | base64
来源：http://rxf.pycfn.com

[R70] 时间戳与互转
来源：http://ocr.zycfv.cn

date +%s;  date -d @1700000000
来源：http://idn.bjfxy.top

[R71] 日期格式化
来源：http://fyj.nanxinkj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bnd.ivvv.top

[R72] 等待端口就绪
来源：http://tkd.chenzaomai.com

until nc -z localhost 3306; do sleep 1; done
来源：http://pxx.daria6918.cn

[R73] 分割大日志
来源：http://ejr.aibaodan.cn

split -l 1000 big.log part_
来源：http://vbp.sweek.top

[R74] 批量重命名
来源：http://dke.yangfankeji.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hpy.cashguo.top

[R75] 导出环境变量
来源：http://ywm.jiagoushi.top

export PATH="$HOME/bin:$PATH"
来源：http://spo.ctjpmb.com

[R76] 使用临时文件
来源：http://kia.c1oappe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bwl.xylfe.cn

[R77] 读取用户输入
来源：http://bag.pengpengdd.cyou

read -rp "请输入: " ans
来源：http://evp.jyoumei.cn

[R78] 交互式菜单
来源：http://iil.9152youxi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oxt.chenjidiqi.icu

[R79] 解析命令行选项
来源：http://tkr.hcnkem.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ilz.jinghuilouyu.cn

[R80] 查看脚本执行耗时
来源：http://mbj.shanyushiyangtech.top

time ./run.sh
来源：http://whj.shzxlz.cn

================================================================================
来源：http://fab.bbcook.cn

S. C / C++ 专题
来源：http://rpk.xuetiantiany.cn

================================================================================
来源：http://fuw.guannengcc.top

[S01] C：Hello World
来源：http://huf.tanke756.top

#include <stdio.h>
来源：http://duc.jyoumei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jif.havefunace.top

[S02] C：变量与格式化输出
来源：http://uud.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://asb.guannengcc.top

[S03] C：读入整数
来源：http://zih.sweek.top

int x; scanf("%d", &x);
来源：http://fvw.nanxuanxn.top

[S04] C：字符串复制
来源：http://ehf.xuanzx.com

char dst[32]; strcpy(dst, "hi");
来源：http://rwy.fanxiaobao.xyz

[S05] C：字符串长度
来源：http://atu.jinghuilouyu.cn

strlen(s)
来源：http://rha.hnxiangtu.top

[S06] C：字符串比较
来源：http://joe.yj20258.top

strcmp(a, b) == 0
来源：http://moz.hywenlv.cn

[S07] C：数组遍历求和
来源：http://sgx.chenzaomai.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uqj.shanyushiyangtech.top

[S08] C：动态内存分配与释放
来源：http://lly.cheryme.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yrj.52xcode.cn

[S09] C：结构体定义与初始化
来源：http://goc.gaohongyu789.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rjq.andypj.xyz

[S10] C：指针与解引用
来源：http://ihc.tianlin.xyz

int *p = &a;  *p = 5;
来源：http://sym.yfazqb.com

[S11] C：逐行读文件
来源：http://wdb.ehwqpu.com

FILE *f = fopen("a.txt", "r");
来源：http://stu.fengsongda.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qni.jinqigfzy.top

fclose(f);
来源：http://rxx.zhaomingkeji.xyz

[S12] C：写文件
来源：http://ugn.gotoacloud.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wzw.hysaishi.cn

[S13] C：宏定义
来源：http://cis.uphjek.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://veu.jinyuanbaomall.cn

[S14] C：枚举
来源：http://oki.gaohongyu789.top

enum Color { RED, GREEN, BLUE };
来源：http://nbo.gotoacloud.top

[S15] C：类型转换
来源：http://izw.0kj1m.cn

(double) a / b
来源：http://vhf.zhoulong.xyz

[S16] C：位操作置位
来源：http://izx.jlsjyb.cn

x |= (1 << 3);
来源：http://kkd.ivvv.top

[S17] C：安全拼接字符串
来源：http://czd.jlsjyb.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pir.nanxuanxn.top

[S18] C：命令行参数
来源：http://cab.gzhubu.top

int main(int argc, char **argv)
来源：http://uvr.ppjwa.cn

[S19] C：快速排序
来源：http://moa.aizwys.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ggi.jqgufenzy.top

[S20] C：二分查找
来源：http://ptt.iojbl.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://krs.nanxinkj.top

[S21] C：字符类别判断
来源：http://ndf.ydzc1.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rmo.tarul.cn

[S22] C：字符串转数字
来源：http://ujh.ehwqpu.com

atoi("42");  strtod("3.14", NULL);
来源：http://foa.shangyingyoupin.top

[S23] C：随机数
来源：http://mrv.shangyingyoupin.top

srand(time(NULL));  int r = rand() % 100;
来源：http://gme.xuanzx.com

[S24] C：获取本地时间
来源：http://tfu.daxiang520.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://way.daxiang520.top

[S25] C：内存拷贝
来源：http://ode.fktsv.cn

memcpy(dst, src, n);
来源：http://khc.aizwys.cn

[S26] C：内存清零
来源：http://bsy.nanxinkj.top

memset(a, 0, sizeof a);
来源：http://tgx.guowangkeji.top

[S27] C：定义常量
来源：http://yzp.zhongyouzk.top

const double PI = 3.14159;
来源：http://bjg.yangfankeji.com

[S28] C：静态变量
来源：http://wjx.shanyushiyangtech.top

static int counter = 0;
来源：http://xry.cdnleiting.top

[S29] C：变参函数
来源：http://qsi.ctjpmb.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fvs.svipenyu.cn

[S30] C：头文件保护
来源：http://snh.ybcxt.top

#ifndef X_H
来源：http://iby.jinyuanbaomall.cn

#define X_H
来源：http://emn.aibaodan.cn

#endif
来源：http://rmz.bbcook.cn

[S31] C++：Hello World
来源：http://ggk.jinyuanbaomall.cn

#include <iostream>
来源：http://mpq.pycfn.com

int main() { std::cout << "Hello\n"; }
来源：http://sep.shanyushiyangtech.top

[S32] C++：字符串
来源：http://iof.ppjwa.cn

std::string s = "hi";  s += "!";
来源：http://tog.uphjek.com

[S33] C++：vector 增删
来源：http://kca.dashuyun.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fhj.shuidangran.top

[S34] C++：遍历 vector
来源：http://emd.fengsongda.top

for (auto &x : v) { std::cout << x; }
来源：http://klx.gotoacloud.top

[S35] C++：map
来源：http://tih.havefunace.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mbg.yvedp.cn

[S36] C++：unordered_map
来源：http://tqt.ppjwa.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nyg.hongshengwenyu.top

[S37] C++：set
来源：http://mhd.kuanghao11.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://anp.pengpengdd.cyou

[S38] C++：排序
来源：http://hha.cashguo.top

std::sort(v.begin(), v.end());
来源：http://lje.dianchejie.cn

[S39] C++：自定义比较器排序
来源：http://yow.redwolf501.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sbk.jyoumei.cn

[S40] C++：查找元素
来源：http://lmj.shanyushiyangtech.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nhy.yfazqb.com

[S41] C++：类与构造函数
来源：http://hqu.tianlin.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gez.cqqwz.cn

[S42] C++：继承与虚函数
来源：http://zbz.jinyuanbaomall.cn

class B : public Base { public: void f() override {} };
来源：http://aft.ehwqpu.com

[S43] C++：智能指针
来源：http://vzs.yuxming.cn

auto p = std::make_unique<int>(5);
来源：http://drg.sysykeji.top

[S44] C++：引用传参
来源：http://xac.shuidangran.top

void inc(int &x) { ++x; }
来源：http://ivd.guannengcc.top

[S45] C++：lambda
来源：http://com.vehdjk.com

auto add = [](int a, int b) { return a + b; };
来源：http://jjj.ydzc1.top

[S46] C++：函数模板
来源：http://adz.ctjpmb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zgj.gotoacloud.top

[S47] C++：结构化绑定遍历
来源：http://owd.jinghuilouyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nsk.yonumen.top

[S48] C++：逐行读文件
来源：http://jwx.shangyingyoupin.top

std::ifstream in("a.txt");  std::string line;
来源：http://hta.wangdashe.top

while (std::getline(in, line)) { }
来源：http://yhd.xylfe.cn

[S49] C++：写文件
来源：http://ddo.dianchejie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://omv.316326.xyz

[S50] C++：格式化数字
来源：http://qhv.jinqigufen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vhe.yuanzhike.top

[S51] C++：显式类型转换
来源：http://dar.jianghu66.top

static_cast<double>(a) / b
来源：http://otc.hywenlv.cn

[S52] C++：const 与 noexcept
来源：http://cqg.nwbrower.top

int size() const noexcept { return n_; }
来源：http://uwe.chenlongwang.top

[S53] C++：移动语义
来源：http://zwf.hongshengwenyu.top

std::vector<int> w = std::move(v);
来源：http://ocs.zdqjudy.top

[S54] C++：异常处理
来源：http://tbp.gaohongyu789.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pbb.cashguo.top

[S55] C++：结构化绑定
来源：http://suo.iojbl.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pvn.quarkkingdee.top

[S56] C++：optional
来源：http://jcw.ydjk.org.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gsq.hysaishi.cn

[S57] C++：编译期常量
来源：http://rzm.dianchejie.cn

constexpr int N = 10;
来源：http://xyv.yfazqb.com

[S58] C++：命名空间
来源：http://kcr.nanxinkj.top

namespace ns { int f() { return 1; } }
来源：http://kzi.chenzaomai.com

[S59] C++：静态断言
来源：http://sun.iojbl.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rls.nanxinkj.top

[S60] C++：遍历并删除元素
来源：http://njt.9152youxi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yvh.jqgufenzy.top

================================================================================
来源：http://pzu.guannengcc.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rrs.ybcxt.top

================================================================================
来源：http://izi.tanke756.top

[T01] Kotlin：Hello World
来源：http://ufe.iojbl.cn

println("Hello")
来源：http://ewq.yueranfly.top

[T02] Kotlin：变量
来源：http://pit.jiagoushi.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sow.gaohongyu789.top

[T03] Kotlin：字符串模板
来源：http://udw.cheryme.top

"值: $b"
来源：http://yyg.meibo888.top

[T04] Kotlin：空安全
来源：http://pvt.hysaishi.cn

val n: String? = null;  n?.length
来源：http://fwa.fehbvm.com


<!-- 参考信息 -->