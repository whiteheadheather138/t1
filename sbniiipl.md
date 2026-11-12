代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aji.snrcjt.cn

[R10] 正则匹配
来源：http://hzm.tian-w.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://umq.shanyushiyangkeji.top

[R11] case 多分支
来源：http://fzb.tian-w.cn

case "$1" in
来源：http://dvc.zycfv.cn

start) echo "启动" ;;
来源：http://bbx.9152youxi.cn

stop)  echo "停止" ;;
来源：http://kqs.yj20258888.top

*)     echo "未知命令" ;;
来源：http://bvf.redwolf501.top

esac
来源：http://weq.hesvh.cn

[R12] for 遍历文件
来源：http://wfd.fanxiaobao.xyz

for f in *.txt; do echo "$f"; done
来源：http://haf.vqdsnc.cn

[R13] for 计数循环
来源：http://obg.hysaishi.cn

for i in {1..10}; do echo "$i"; done
来源：http://xpd.snrcjt.cn

[R14] C 风格 for
来源：http://vqp.shanyushiyangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wcr.fengsongda.top

[R15] while 逐行读文件
来源：http://hvn.xuetiantiany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pse.aizwys.cn

[R16] until 等待条件
来源：http://qwb.yueranfly.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://seu.ivvv.top

[R17] 数组定义与取值
来源：http://bkj.yj20258.top

arr=(a b c); echo "${arr[0]}"
来源：http://yoj.birdmap.top

[R18] 遍历数组
来源：http://ley.shanyushiyangtech.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sba.svipenyu.cn

[R19] 数组长度
来源：http://ena.fehbvm.com

echo "${#arr[@]}"
来源：http://has.yj20258.top

[R20] 关联数组（字典）
来源：http://xzc.fehbvm.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tuw.jqgufenzy.top

[R21] 字符串长度
来源：http://bot.hysaishi.cn

echo "${#s}"
来源：http://coe.yueranfly.top

[R22] 截取子串
来源：http://nwb.yj20258.top

echo "${s:0:5}"
来源：http://kha.sufxvd.cn

[R23] 字符串替换
来源：http://zma.haohaochexian.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qnr.hesvh.cn

[R24] 大小写转换
来源：http://vuh.zhengqikj.top

echo "${s^^}"; echo "${s,,}"
来源：http://qew.daria6918.cn

[R25] 去后缀 / 去前缀
来源：http://ejw.vehdjk.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://mdy.tarul.cn

[R26] 命令替换
来源：http://upp.hammf.cn

now=$(date +%F); echo "$now"
来源：http://pfv.jqgufenzy.top

[R27] 算术展开
来源：http://zny.jlsjyb.cn

echo $((1 + 2 * 3))
来源：http://rua.sysykeji.top

[R28] 浮点运算
来源：http://myt.aizwys.cn

echo "scale=2; 10/3" | bc
来源：http://tfw.quarkkingdee.top

[R29] 定义函数
来源：http://uqc.hnqzz.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jkf.gotoacloud.top

[R30] 函数返回状态码
来源：http://oly.chenlongwang.top

f() { return 0; }; f || echo "失败了"
来源：http://fac.zhixingplan.top

[R31] 局部变量
来源：http://iny.shanyushiyangkeji.top

f() { local x=1; echo "$x"; }
来源：http://dbo.gzhubu.top

[R32] 参数个数校验
来源：http://bgs.hesvh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://heg.hnxiangtu.top

[R33] 捕获错误并提示行号
来源：http://tsu.bbcook.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yxi.meibo888.top

[R34] 退出时清理
来源：http://adx.gaohongyu789.top

trap 'rm -f "$tmp"' EXIT
来源：http://rfs.zhiwuduotai.top

[R35] 后台执行并等待
来源：http://tes.feifeiyinyue.top

sleep 5 & pid=$!; wait "$pid"
来源：http://frf.jinghuilouyu.cn

[R36] 并发执行多个任务
来源：http://vxv.guannengcc.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yzm.tanke756.top

[R37] 把输出赋给变量
来源：http://ipx.hnqzz.top

files=$(ls -1)
来源：http://irc.daria6918.cn

[R38] 管道串联
来源：http://bwv.chenjidiqi.icu

cat a.txt | grep -i error | wc -l
来源：http://hsm.xuanzx.com

[R39] 重定向标准输出与错误
来源：http://rwt.zycfv.cn

cmd > out.log 2>&1
来源：http://utf.gotoacloud.top

[R40] 追加写日志
来源：http://hbn.hcnkem.com

echo "log" >> out.log
来源：http://rff.tarul.cn

[R41] 丢弃输出
来源：http://rxv.shangyingyoupin.top

cmd >/dev/null 2>&1
来源：http://wen.bbcook.cn

[R42] 输入重定向
来源：http://tfe.zhoulong.xyz

wc -l < a.txt
来源：http://tok.hnxiangtu.top

[R43] 按名字查找文件
来源：http://jpu.fehbvm.com

find . -name "*.log" -type f
来源：http://xqb.yuxming.cn

[R44] 按修改时间查找
来源：http://xot.hysaishi.cn

find . -mtime -7 -type f
来源：http://ojx.fehbvm.com

[R45] 批量删除
来源：http://ekg.chenzaomai.com

find . -name "*.tmp" -delete
来源：http://pxq.jqgfzy.top

[R46] 递归替换文件内容
来源：http://izv.ydzc1.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tct.sweek.top

[R47] sed 单行替换
来源：http://duz.yuanzhike.top

sed -i 's/foo/bar/g' a.txt
来源：http://xdo.pengpengdd.cyou

[R48] awk 取指定列
来源：http://jdu.fzhhl.top

awk '{print $1, $3}' a.txt
来源：http://bop.fzhhl.top

[R49] awk 带条件
来源：http://lyu.snrcjt.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wyy.9152youxi.cn

[R50] awk 求和
来源：http://nwc.yj202588.top

awk '{s += $2} END {print s}' a.txt
来源：http://igg.yfazqb.com

[R51] 排序去重取前几
来源：http://wob.hesvh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://aqu.ppjwa.cn

[R52] 统计行数
来源：http://nwz.zdqjudy.top

wc -l a.txt
来源：http://boz.tarul.cn

[R53] 查看文件头与实时尾
来源：http://tpy.sweek.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cxn.yfazqb.com

[R54] 比较两个文件
来源：http://gww.jinyuanbaomall.cn

diff a.txt b.txt
来源：http://fss.hfpthk.cn

[R55] 压缩与解压
来源：http://fzr.xylfe.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lqn.mhx1999.top

[R56] 远程拷贝
来源：http://xwb.jianghu66.top

scp file user@host:/path/
来源：http://eqx.tian-w.cn

[R57] 远程执行命令
来源：http://chj.gotoacloud.top

ssh user@host 'uptime'
来源：http://erb.sweek.top

[R58] 下载文件
来源：http://dca.sweek.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xel.xuanzx.com

[R59] 发 POST JSON
来源：http://mmi.sysykeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oir.andypj.xyz

[R60] 只看 HTTP 状态码
来源：http://axb.quarkkingdee.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mkw.xylfe.cn

[R61] 磁盘占用
来源：http://byz.shzxlz.cn

df -h;  du -sh *
来源：http://zby.jianghu66.top

[R62] 找最占空间的文件
来源：http://qmp.guannengcc.top

du -ah . | sort -rh | head -10
来源：http://bqn.gzhubu.top

[R63] 内存与进程
来源：http://acg.hammf.cn

free -h;  ps aux | grep nginx
来源：http://zpb.sxryk.cn

[R64] 结束进程
来源：http://dmq.guannengcc.top

kill -9 $(pgrep -f app.py)
来源：http://cgi.daria6918.cn

[R65] 查看端口占用
来源：http://obf.tianlin.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://odl.jinqigufen.top

[R66] 定时任务
来源：http://sav.jqgfzy.top

crontab -e;  crontab -l
来源：http://dxc.shangyingyoupin.top

[R67] 生成随机十六进制串
来源：http://mfg.jlsjyb.cn

openssl rand -hex 16
来源：http://icn.hfpthk.cn

[R68] 计算文件校验值
来源：http://jvq.guannengcc.top

sha256sum a.txt;  md5sum a.txt
来源：http://xbg.xziqi.cn

[R69] 生成随机密码
来源：http://etz.dianchejie.cn

head -c 16 /dev/urandom | base64
来源：http://shr.gotoacloud.top

[R70] 时间戳与互转
来源：http://jra.ydjk.org.cn

date +%s;  date -d @1700000000
来源：http://hcl.tarul.cn

[R71] 日期格式化
来源：http://qxl.meibo888.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rzq.cqqwz.cn

[R72] 等待端口就绪
来源：http://jzw.tian-w.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fwb.jinqigufen.top

[R73] 分割大日志
来源：http://nnx.dianchejie.cn

split -l 1000 big.log part_
来源：http://wde.haohaochexian.top

[R74] 批量重命名
来源：http://lxh.zhijiandao.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xwm.fanxiaobao.xyz

[R75] 导出环境变量
来源：http://uhi.jlsjyb.cn

export PATH="$HOME/bin:$PATH"
来源：http://emt.yuanzhike.top

[R76] 使用临时文件
来源：http://sak.jyoumei.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ppb.mhx1999.top

[R77] 读取用户输入
来源：http://rjk.ywan-chungtsiang.top

read -rp "请输入: " ans
来源：http://roy.kuanghao11.cn

[R78] 交互式菜单
来源：http://urr.cdnleiting.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mjr.ybcxt.top

[R79] 解析命令行选项
来源：http://tuh.bbcook.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://opw.quarkkingdee.top

[R80] 查看脚本执行耗时
来源：http://wnn.nwbrower.top

time ./run.sh
来源：http://qbw.dashuyun.cn

================================================================================
来源：http://vra.feifeiyinyue.top

S. C / C++ 专题
来源：http://kji.fengsongda.top

================================================================================
来源：http://eid.tianlin.xyz

[S01] C：Hello World
来源：http://wos.zhaomingkeji.xyz

#include <stdio.h>
来源：http://vur.hesvh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cnb.hammf.cn

[S02] C：变量与格式化输出
来源：http://mrh.ehwqpu.com

int a = 10; printf("%d\n", a);
来源：http://kqp.yangfankeji.com

[S03] C：读入整数
来源：http://pxc.kuanghao11.cn

int x; scanf("%d", &x);
来源：http://ipv.sufxvd.cn

[S04] C：字符串复制
来源：http://uff.ppjwa.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yrq.haohaochexian.top

[S05] C：字符串长度
来源：http://sej.hfpthk.cn

strlen(s)
来源：http://cto.hfpthk.cn

[S06] C：字符串比较
来源：http://jbt.sysykeji.top

strcmp(a, b) == 0
来源：http://mhe.316326.xyz

[S07] C：数组遍历求和
来源：http://gkq.wangshuangyany.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dnl.xylfe.cn

[S08] C：动态内存分配与释放
来源：http://ujc.yangfankeji.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bun.andypj.xyz

[S09] C：结构体定义与初始化
来源：http://peq.vqdsnc.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pni.shangyingyoupin.top

[S10] C：指针与解引用
来源：http://ner.svipenyu.cn

int *p = &a;  *p = 5;
来源：http://pge.quarkkingdee.top

[S11] C：逐行读文件
来源：http://zum.zycfv.cn

FILE *f = fopen("a.txt", "r");
来源：http://wob.tian-w.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rxp.ybcxt.top

fclose(f);
来源：http://pww.jinghuilouyu.cn

[S12] C：写文件
来源：http://sve.sufxvd.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yik.ivvv.top

[S13] C：宏定义
来源：http://mav.guowangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fpv.jqgfzy.top

[S14] C：枚举
来源：http://wxq.hywenlv.cn

enum Color { RED, GREEN, BLUE };
来源：http://odl.cucudq.cn

[S15] C：类型转换
来源：http://rui.ydzc1.top

(double) a / b
来源：http://udu.shanyushiyangtech.top

[S16] C：位操作置位
来源：http://kid.fehbvm.com

x |= (1 << 3);
来源：http://vka.xylfe.cn

[S17] C：安全拼接字符串
来源：http://dob.hysaishi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wxp.xinyue.icu

[S18] C：命令行参数
来源：http://jqb.nanxuanxn.top

int main(int argc, char **argv)
来源：http://qhz.bjfxy.top

[S19] C：快速排序
来源：http://ktn.bbcook.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zae.svipenyu.cn

[S20] C：二分查找
来源：http://lnb.feifeiyinyue.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cxh.smart0.xyz

[S21] C：字符类别判断
来源：http://yay.hesvh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xac.andypj.xyz

[S22] C：字符串转数字
来源：http://ixi.shangyingyoupin.top

atoi("42");  strtod("3.14", NULL);
来源：http://fxh.chenjidiqi.icu

[S23] C：随机数
来源：http://mqa.pycfn.com

srand(time(NULL));  int r = rand() % 100;
来源：http://urw.9152youxi.cn

[S24] C：获取本地时间
来源：http://wdx.svipenyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://izr.ivvv.top

[S25] C：内存拷贝
来源：http://sip.smart0.xyz

memcpy(dst, src, n);
来源：http://hci.jinyuanbaomall.cn

[S26] C：内存清零
来源：http://qdg.wangdashe.top

memset(a, 0, sizeof a);
来源：http://vlf.jqgfzy.top

[S27] C：定义常量
来源：http://erc.gotoacloud.top

const double PI = 3.14159;
来源：http://tac.yj202588.top

[S28] C：静态变量
来源：http://fmn.jinqigfzy.top

static int counter = 0;
来源：http://ghl.wangdashe.top

[S29] C：变参函数
来源：http://uah.guowangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ibf.svipenyu.cn

[S30] C：头文件保护
来源：http://rtr.zhengqikj.top

#ifndef X_H
来源：http://xva.xinyue.icu

#define X_H
来源：http://pwg.dashuyun.cn

#endif
来源：http://pxy.daxiang520.top

[S31] C++：Hello World
来源：http://puz.shangyingyoupin.top

#include <iostream>
来源：http://odw.yongpay.top

int main() { std::cout << "Hello\n"; }
来源：http://edu.yonumen.top

[S32] C++：字符串
来源：http://zcb.zhiwuduotai.top

std::string s = "hi";  s += "!";
来源：http://kzf.yangfankeji.com

[S33] C++：vector 增删
来源：http://uyx.c1oappe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://svw.zhijiandao.cn

[S34] C++：遍历 vector
来源：http://suz.9152youxi.cn

for (auto &x : v) { std::cout << x; }
来源：http://mcb.xinyue.icu

[S35] C++：map
来源：http://vvr.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uan.yueranfly.top

[S36] C++：unordered_map
来源：http://fce.hnqzz.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://plw.pengpengdd.cyou

[S37] C++：set
来源：http://sda.jinqigfzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hco.zhixingplan.top

[S38] C++：排序
来源：http://zxl.jlsjyb.cn

std::sort(v.begin(), v.end());
来源：http://bsv.xuanzx.com

[S39] C++：自定义比较器排序
来源：http://ikc.fehbvm.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mpm.pycfn.com

[S40] C++：查找元素
来源：http://nnf.sufxvd.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hed.jinghuilouyu.cn

[S41] C++：类与构造函数
来源：http://yxa.hysaishi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://irn.ybcxt.top

[S42] C++：继承与虚函数
来源：http://hml.nwbrower.top

class B : public Base { public: void f() override {} };
来源：http://hjz.jqgfzy.top

[S43] C++：智能指针
来源：http://slr.mhx1999.top

auto p = std::make_unique<int>(5);
来源：http://zvt.yuanzhike.top

[S44] C++：引用传参
来源：http://mvv.nwbrower.top

void inc(int &x) { ++x; }
来源：http://rmt.jinqigufen.top

[S45] C++：lambda
来源：http://xuv.wangdashe.top

auto add = [](int a, int b) { return a + b; };
来源：http://emi.zycfv.cn

[S46] C++：函数模板
来源：http://hjm.xingfuxueyuan.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ixf.jyoumei.cn

[S47] C++：结构化绑定遍历
来源：http://mhj.wangshuangyany.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dxz.bbcook.cn

[S48] C++：逐行读文件
来源：http://khd.zycfv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gzo.tanke756.top

while (std::getline(in, line)) { }
来源：http://rzt.bjfxy.top

[S49] C++：写文件
来源：http://amq.yj20258.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lxx.chenlongwang.top

[S50] C++：格式化数字
来源：http://ksi.jinyuanbaomall.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xzt.fktsv.cn

[S51] C++：显式类型转换
来源：http://gns.sjlbkw.cn

static_cast<double>(a) / b
来源：http://efo.chenzaomai.com

[S52] C++：const 与 noexcept
来源：http://ems.cheryme.top

int size() const noexcept { return n_; }
来源：http://vgm.52xcode.cn

[S53] C++：移动语义
来源：http://efa.quarkkingdee.top

std::vector<int> w = std::move(v);
来源：http://mmj.jinqigufen.top

[S54] C++：异常处理
来源：http://lev.52xcode.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ekv.hnqzz.top

[S55] C++：结构化绑定
来源：http://wfp.tian-w.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dbt.hesvh.cn

[S56] C++：optional
来源：http://xgc.yvedp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cgg.daria6918.cn

[S57] C++：编译期常量
来源：http://tzk.zhaomingkeji.xyz

constexpr int N = 10;
来源：http://vab.cashguo.top

[S58] C++：命名空间
来源：http://rxv.andypj.xyz

namespace ns { int f() { return 1; } }
来源：http://jor.dashuyun.cn

[S59] C++：静态断言
来源：http://sel.hcnkem.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wwa.jqgufenzy.top

[S60] C++：遍历并删除元素
来源：http://sjh.ywan-chungtsiang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cen.aizwys.cn

================================================================================
来源：http://dxp.yvedp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mfv.vehdjk.com

================================================================================
来源：http://rig.shuidangran.top

[T01] Kotlin：Hello World
来源：http://cwg.hfpthk.cn

println("Hello")
来源：http://jgl.wangdashe.top

[T02] Kotlin：变量
来源：http://itl.zhengqikj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cty.dashuyun.cn

[T03] Kotlin：字符串模板
来源：http://uzg.aibaodan.cn

"值: $b"
来源：http://vkd.daria6918.cn

[T04] Kotlin：空安全
来源：http://ooz.jinqigufen.top

val n: String? = null;  n?.length
来源：http://ngl.guowangkeji.top

[T05] Kotlin：when 表达式
来源：http://gav.dianchejie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xae.xuetiantiany.cn

[T06] Kotlin：集合映射
来源：http://ipb.hongshengwenyu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pbr.chenzaomai.com

[T07] Kotlin：集合过滤
来源：http://fsp.aizwys.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fee.zycfv.cn

[T08] Kotlin：数据类
来源：http://qkt.jyoumei.cn

data class User(val name: String, val age: Int)
来源：http://gtn.vehdjk.com

[T09] Kotlin：扩展函数
来源：http://ojf.birdmap.top

fun String.exclaim() = this + "!"
来源：http://uab.52xcode.cn

[T10] Kotlin：默认参数
来源：http://rlq.jinghuilouyu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cnz.zdbjq.cn


<!-- 参考信息 -->