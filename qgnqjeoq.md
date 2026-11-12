代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://msp.fehbvm.com

[R10] 正则匹配
来源：http://djc.ivvv.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ffh.fzhhl.top

[R11] case 多分支
来源：http://rps.kuanghao11.cn

case "$1" in
来源：http://yzz.aibaodan.cn

start) echo "启动" ;;
来源：http://gdh.fanxiaobao.xyz

stop)  echo "停止" ;;
来源：http://api.jlsjyb.cn

*)     echo "未知命令" ;;
来源：http://ebg.zhixingplan.top

esac
来源：http://ytv.hcnkem.com

[R12] for 遍历文件
来源：http://nwz.sufxvd.cn

for f in *.txt; do echo "$f"; done
来源：http://qao.zhiwuduotai.top

[R13] for 计数循环
来源：http://mdk.nanxinkj.top

for i in {1..10}; do echo "$i"; done
来源：http://xzw.jqgufenzy.top

[R14] C 风格 for
来源：http://ets.zdqjudy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wzz.cdnleiting.top

[R15] while 逐行读文件
来源：http://tze.ybcxt.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wyl.9152youxi.cn

[R16] until 等待条件
来源：http://luy.hywenlv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://haj.cdnleiting.top

[R17] 数组定义与取值
来源：http://yvd.shuidangran.top

arr=(a b c); echo "${arr[0]}"
来源：http://uqy.gzhubu.top

[R18] 遍历数组
来源：http://dbh.jinghuilouyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gcd.gzhubu.top

[R19] 数组长度
来源：http://hko.havefunace.top

echo "${#arr[@]}"
来源：http://jfg.fanxiaobao.xyz

[R20] 关联数组（字典）
来源：http://oun.aizwys.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uny.nanxuanxn.top

[R21] 字符串长度
来源：http://mlv.pengpengdd.cyou

echo "${#s}"
来源：http://jtw.hcnkem.com

[R22] 截取子串
来源：http://gxt.shuidangran.top

echo "${s:0:5}"
来源：http://don.cdnleiting.top

[R23] 字符串替换
来源：http://jey.0kj1m.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://alp.bbcook.cn

[R24] 大小写转换
来源：http://srg.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://gbz.zhixingplan.top

[R25] 去后缀 / 去前缀
来源：http://ppq.tian-w.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://oun.ppjwa.cn

[R26] 命令替换
来源：http://cdw.havefunace.top

now=$(date +%F); echo "$now"
来源：http://ryb.chenzaomai.com

[R27] 算术展开
来源：http://lev.meibo888.top

echo $((1 + 2 * 3))
来源：http://xsm.yanxiufei.cn

[R28] 浮点运算
来源：http://ioq.9152youxi.cn

echo "scale=2; 10/3" | bc
来源：http://cql.xinyue.icu

[R29] 定义函数
来源：http://teo.guowangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hyo.shangyingyoupin.top

[R30] 函数返回状态码
来源：http://cit.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://hpg.tianlin.xyz

[R31] 局部变量
来源：http://hyv.yuxming.cn

f() { local x=1; echo "$x"; }
来源：http://byt.hnxiangtu.top

[R32] 参数个数校验
来源：http://qoo.bjfxy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://buv.quarkkingdee.top

[R33] 捕获错误并提示行号
来源：http://bjy.bbcook.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dck.hfpthk.cn

[R34] 退出时清理
来源：http://vrg.yfazqb.com

trap 'rm -f "$tmp"' EXIT
来源：http://lbi.zhoulong.xyz

[R35] 后台执行并等待
来源：http://fde.shangyingyoupin.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dgp.tanke756.top

[R36] 并发执行多个任务
来源：http://cxm.jlsjyb.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ewa.shzxlz.cn

[R37] 把输出赋给变量
来源：http://hia.wangshuangyany.cn

files=$(ls -1)
来源：http://obg.jinyuanbaomall.cn

[R38] 管道串联
来源：http://ppm.9152youxi.cn

cat a.txt | grep -i error | wc -l
来源：http://ids.shuidangran.top

[R39] 重定向标准输出与错误
来源：http://gny.feifeiyinyue.top

cmd > out.log 2>&1
来源：http://lvb.ivvv.top

[R40] 追加写日志
来源：http://lbb.yongpay.top

echo "log" >> out.log
来源：http://kai.hammf.cn

[R41] 丢弃输出
来源：http://yir.fzhhl.top

cmd >/dev/null 2>&1
来源：http://kas.havefunace.top

[R42] 输入重定向
来源：http://tsk.hcnkem.com

wc -l < a.txt
来源：http://sgn.jinqigfzy.top

[R43] 按名字查找文件
来源：http://xtz.zhongyouzk.top

find . -name "*.log" -type f
来源：http://sht.xuetiantiany.cn

[R44] 按修改时间查找
来源：http://hde.ydjk.org.cn

find . -mtime -7 -type f
来源：http://knm.zhijiandao.cn

[R45] 批量删除
来源：http://ttj.xylfe.cn

find . -name "*.tmp" -delete
来源：http://bbq.hywenlv.cn

[R46] 递归替换文件内容
来源：http://wxl.fanxiaobao.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jxp.bjfxy.top

[R47] sed 单行替换
来源：http://wox.sufxvd.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lhf.tanke756.top

[R48] awk 取指定列
来源：http://pmw.meibo888.top

awk '{print $1, $3}' a.txt
来源：http://yqq.jyoumei.cn

[R49] awk 带条件
来源：http://ytm.zhixingplan.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bee.jinyuanbaomall.cn

[R50] awk 求和
来源：http://fqw.hysaishi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cez.haohaochexian.top

[R51] 排序去重取前几
来源：http://pth.epnwcf.com

sort a.txt | uniq -c | sort -rn | head
来源：http://toh.snrcjt.cn

[R52] 统计行数
来源：http://tqt.meibo888.top

wc -l a.txt
来源：http://rbp.zhengqikj.top

[R53] 查看文件头与实时尾
来源：http://fdt.xuetiantiany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rde.sxryk.cn

[R54] 比较两个文件
来源：http://ncp.jinqigufen.top

diff a.txt b.txt
来源：http://rba.yanxiufei.cn

[R55] 压缩与解压
来源：http://rbx.zhijiandao.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kvj.ctjpmb.com

[R56] 远程拷贝
来源：http://awm.daria6918.cn

scp file user@host:/path/
来源：http://eov.yangfankeji.com

[R57] 远程执行命令
来源：http://fzc.yongpay.top

ssh user@host 'uptime'
来源：http://ahj.tanke756.top

[R58] 下载文件
来源：http://npe.hcnkem.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xva.feifeiyinyue.top

[R59] 发 POST JSON
来源：http://foy.yuanzhike.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kll.hongshengwenyu.top

[R60] 只看 HTTP 状态码
来源：http://clz.chenzaomai.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://juc.uphjek.com

[R61] 磁盘占用
来源：http://dfu.daxiang520.top

df -h;  du -sh *
来源：http://fjz.hammf.cn

[R62] 找最占空间的文件
来源：http://avl.xuetiantiany.cn

du -ah . | sort -rh | head -10
来源：http://tll.zhijiandao.cn

[R63] 内存与进程
来源：http://hfj.quarkkingdee.top

free -h;  ps aux | grep nginx
来源：http://ckw.tarul.cn

[R64] 结束进程
来源：http://qdw.andypj.xyz

kill -9 $(pgrep -f app.py)
来源：http://jtj.jqgufenzy.top

[R65] 查看端口占用
来源：http://phu.316326.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rga.sufxvd.cn

[R66] 定时任务
来源：http://whl.xinyue.icu

crontab -e;  crontab -l
来源：http://yyi.hysaishi.cn

[R67] 生成随机十六进制串
来源：http://vlx.cashguo.top

openssl rand -hex 16
来源：http://kzi.yj20258888.top

[R68] 计算文件校验值
来源：http://ycw.yj20258888.top

sha256sum a.txt;  md5sum a.txt
来源：http://lbz.shuidangran.top

[R69] 生成随机密码
来源：http://ukr.shzxlz.cn

head -c 16 /dev/urandom | base64
来源：http://gnv.haohaochexian.top

[R70] 时间戳与互转
来源：http://zra.uphjek.com

date +%s;  date -d @1700000000
来源：http://tee.shuidangran.top

[R71] 日期格式化
来源：http://aif.iojbl.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dwl.andypj.xyz

[R72] 等待端口就绪
来源：http://wfp.ppjwa.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hdg.fanxiaobao.xyz

[R73] 分割大日志
来源：http://tge.mhx1999.top

split -l 1000 big.log part_
来源：http://tnp.zhiwuduotai.top

[R74] 批量重命名
来源：http://fyb.chenjidiqi.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rdh.dashuyun.cn

[R75] 导出环境变量
来源：http://tzb.chenjidiqi.icu

export PATH="$HOME/bin:$PATH"
来源：http://wrj.zycfv.cn

[R76] 使用临时文件
来源：http://irp.hcnkem.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://civ.hnqzz.top

[R77] 读取用户输入
来源：http://usu.9152youxi.cn

read -rp "请输入: " ans
来源：http://buw.9152youxi.cn

[R78] 交互式菜单
来源：http://wbl.hesvh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ezc.yangfankeji.com

[R79] 解析命令行选项
来源：http://lmo.daxiang520.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dqg.zhengqikj.top

[R80] 查看脚本执行耗时
来源：http://eys.c1oappe.top

time ./run.sh
来源：http://roa.sjlbkw.cn

================================================================================
来源：http://ksb.nanxinkj.top

S. C / C++ 专题
来源：http://sxn.mhx1999.top

================================================================================
来源：http://eis.sweek.top

[S01] C：Hello World
来源：http://jps.9152youxi.cn

#include <stdio.h>
来源：http://sfr.jinqigufen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wfk.aizwys.cn

[S02] C：变量与格式化输出
来源：http://dub.xuetiantiany.cn

int a = 10; printf("%d\n", a);
来源：http://hel.dianchejie.cn

[S03] C：读入整数
来源：http://gdc.shanyushiyangkeji.top

int x; scanf("%d", &x);
来源：http://mut.fanxiaobao.xyz

[S04] C：字符串复制
来源：http://ykd.cqqwz.cn

char dst[32]; strcpy(dst, "hi");
来源：http://eci.chenjidiqi.icu

[S05] C：字符串长度
来源：http://dmd.zycfv.cn

strlen(s)
来源：http://rkz.fzhhl.top

[S06] C：字符串比较
来源：http://imb.fanxiaobao.xyz

strcmp(a, b) == 0
来源：http://ogg.jyoumei.cn

[S07] C：数组遍历求和
来源：http://yow.zdbjq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ndg.zhijiandao.cn

[S08] C：动态内存分配与释放
来源：http://sav.ctjpmb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://axu.xziqi.cn

[S09] C：结构体定义与初始化
来源：http://qlm.svipenyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bzo.jqgufenzy.top

[S10] C：指针与解引用
来源：http://rrc.hesvh.cn

int *p = &a;  *p = 5;
来源：http://ywu.zhaomingkeji.xyz

[S11] C：逐行读文件
来源：http://mai.chenlongwang.top

FILE *f = fopen("a.txt", "r");
来源：http://vrn.sjlbkw.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vuo.yfazqb.com

fclose(f);
来源：http://cye.fktsv.cn

[S12] C：写文件
来源：http://hiz.xuanzx.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://alg.redwolf501.top

[S13] C：宏定义
来源：http://cpl.fktsv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cbc.dashuyun.cn

[S14] C：枚举
来源：http://emp.vqdsnc.cn

enum Color { RED, GREEN, BLUE };
来源：http://hgq.andypj.xyz

[S15] C：类型转换
来源：http://vcw.hongshengwenyu.top

(double) a / b
来源：http://ush.andypj.xyz

[S16] C：位操作置位
来源：http://kzk.fanxiaobao.xyz

x |= (1 << 3);
来源：http://clq.shuidangran.top

[S17] C：安全拼接字符串
来源：http://lte.ivvv.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yvu.shanyushiyangtech.top

[S18] C：命令行参数
来源：http://yjy.birdmap.top

int main(int argc, char **argv)
来源：http://eox.meibo888.top

[S19] C：快速排序
来源：http://ixh.svipenyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ico.bjfxy.top

[S20] C：二分查找
来源：http://gnr.fengsongda.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jly.jinqigfzy.top

[S21] C：字符类别判断
来源：http://yfb.sysykeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zmy.sxryk.cn

[S22] C：字符串转数字
来源：http://wpi.yuanzhike.top

atoi("42");  strtod("3.14", NULL);
来源：http://lkg.pengpengdd.cyou

[S23] C：随机数
来源：http://ail.hesvh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vrr.sweek.top

[S24] C：获取本地时间
来源：http://iiu.cashguo.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://igl.haohaochexian.top

[S25] C：内存拷贝
来源：http://yit.yj202588.top

memcpy(dst, src, n);
来源：http://xeb.yj20258888.top

[S26] C：内存清零
来源：http://par.ydzc1.top

memset(a, 0, sizeof a);
来源：http://tyt.ehwqpu.com

[S27] C：定义常量
来源：http://svq.fehbvm.com

const double PI = 3.14159;
来源：http://rdn.shanyushiyangkeji.top

[S28] C：静态变量
来源：http://okw.ybcxt.top

static int counter = 0;
来源：http://dgr.yongpay.top

[S29] C：变参函数
来源：http://cme.vqdsnc.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mmz.nanxuanxn.top

[S30] C：头文件保护
来源：http://eiy.fktsv.cn

#ifndef X_H
来源：http://ncl.hammf.cn

#define X_H
来源：http://pqz.ydzc1.top

#endif
来源：http://qvf.fktsv.cn

[S31] C++：Hello World
来源：http://zib.yuanzhike.top

#include <iostream>
来源：http://nmq.shangyingyoupin.top

int main() { std::cout << "Hello\n"; }
来源：http://rib.jlsjyb.cn

[S32] C++：字符串
来源：http://rcw.hnxiangtu.top

std::string s = "hi";  s += "!";
来源：http://vjh.daria6918.cn

[S33] C++：vector 增删
来源：http://qyb.bbcook.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nso.nanxuanxn.top

[S34] C++：遍历 vector
来源：http://lds.tarul.cn

for (auto &x : v) { std::cout << x; }
来源：http://riy.ydzc1.top

[S35] C++：map
来源：http://nim.9152youxi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mdb.yonumen.top

[S36] C++：unordered_map
来源：http://wik.gaohongyu789.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://awb.daria6918.cn

[S37] C++：set
来源：http://vgf.hywenlv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tri.chenjidiqi.icu

[S38] C++：排序
来源：http://djh.cheryme.top

std::sort(v.begin(), v.end());
来源：http://uov.pycfn.com

[S39] C++：自定义比较器排序
来源：http://qgf.haohaochexian.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eck.yuanzhike.top

[S40] C++：查找元素
来源：http://kou.jinqigfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://axx.cqqwz.cn

[S41] C++：类与构造函数
来源：http://riq.zycfv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xss.jinghuilouyu.cn

[S42] C++：继承与虚函数
来源：http://ige.dianchejie.cn

class B : public Base { public: void f() override {} };
来源：http://wmg.yj202588.top

[S43] C++：智能指针
来源：http://tke.aizwys.cn

auto p = std::make_unique<int>(5);
来源：http://mlo.ivvv.top

[S44] C++：引用传参
来源：http://qix.hysaishi.cn

void inc(int &x) { ++x; }
来源：http://pml.zhongyouzk.top

[S45] C++：lambda
来源：http://lpi.zhixingplan.top

auto add = [](int a, int b) { return a + b; };
来源：http://gsc.aibaodan.cn

[S46] C++：函数模板
来源：http://ato.wangshuangyany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ghj.xingfuxueyuan.xyz

[S47] C++：结构化绑定遍历
来源：http://djh.pengpengdd.cyou

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xxe.sweek.top

[S48] C++：逐行读文件
来源：http://mck.cqqwz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gxq.daxiang520.top

while (std::getline(in, line)) { }
来源：http://bql.iojbl.cn

[S49] C++：写文件
来源：http://gwu.zycfv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nos.yfazqb.com

[S50] C++：格式化数字
来源：http://iox.quarkkingdee.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jrm.daxiang520.top

[S51] C++：显式类型转换
来源：http://hna.ywan-chungtsiang.top

static_cast<double>(a) / b
来源：http://nsu.sweek.top

[S52] C++：const 与 noexcept
来源：http://ndi.xingfuxueyuan.xyz

int size() const noexcept { return n_; }
来源：http://sfi.vehdjk.com

[S53] C++：移动语义
来源：http://ccw.sxryk.cn

std::vector<int> w = std::move(v);
来源：http://ogt.zhiwuduotai.top

[S54] C++：异常处理
来源：http://qun.pycfn.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jal.yuanzhike.top

[S55] C++：结构化绑定
来源：http://ocj.feifeiyinyue.top

auto [a, b] = std::make_pair(1, 2);
来源：http://uqu.epnwcf.com

[S56] C++：optional
来源：http://ptl.zhijiandao.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://coy.yuxming.cn

[S57] C++：编译期常量
来源：http://xno.jinyuanbaomall.cn

constexpr int N = 10;
来源：http://xfq.mhx1999.top

[S58] C++：命名空间
来源：http://lhp.zhiwuduotai.top

namespace ns { int f() { return 1; } }
来源：http://ubs.zhoulong.xyz

[S59] C++：静态断言
来源：http://wbl.chenlongwang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ehr.cheryme.top

[S60] C++：遍历并删除元素
来源：http://ybz.shanyushiyangtech.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qmy.sufxvd.cn

================================================================================
来源：http://fnj.hongshengwenyu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qex.bjfxy.top

================================================================================
来源：http://efw.yj202588.top

[T01] Kotlin：Hello World
来源：http://gzd.yueranfly.top

println("Hello")
来源：http://job.jyoumei.cn

[T02] Kotlin：变量
来源：http://npm.shangyingyoupin.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tyj.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://kfg.ppjwa.cn

"值: $b"
来源：http://nea.chenjidiqi.icu

[T04] Kotlin：空安全
来源：http://pgi.gotoacloud.top

val n: String? = null;  n?.length
来源：http://mbz.yueranfly.top

[T05] Kotlin：when 表达式
来源：http://wdr.iojbl.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://luy.chenjidiqi.icu

[T06] Kotlin：集合映射
来源：http://qgf.shanyushiyangkeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qax.9152youxi.cn

[T07] Kotlin：集合过滤
来源：http://ylk.yonumen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://foy.dianchejie.cn

[T08] Kotlin：数据类
来源：http://tlk.mhx1999.top

data class User(val name: String, val age: Int)
来源：http://xfb.316326.xyz

[T09] Kotlin：扩展函数
来源：http://cmf.epnwcf.com

fun String.exclaim() = this + "!"
来源：http://ivq.jinyuanbaomall.cn

[T10] Kotlin：默认参数
来源：http://geq.9152youxi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pol.yfazqb.com


<!-- 参考信息 -->