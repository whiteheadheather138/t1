代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gft.fanxiaobao.xyz

[R10] 正则匹配
来源：http://vxu.jqgufenzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bbk.xziqi.cn

[R11] case 多分支
来源：http://tmu.gogol.net.cn

case "$1" in
来源：http://zqg.cheryme.top

start) echo "启动" ;;
来源：http://igm.ybcxt.top

stop)  echo "停止" ;;
来源：http://fex.xinyue.icu

*)     echo "未知命令" ;;
来源：http://bmz.hesvh.cn

esac
来源：http://jbl.yfazqb.com

[R12] for 遍历文件
来源：http://jgn.hfpthk.cn

for f in *.txt; do echo "$f"; done
来源：http://lou.birdmap.top

[R13] for 计数循环
来源：http://imz.fanxiaobao.xyz

for i in {1..10}; do echo "$i"; done
来源：http://xfp.jqgufenzy.top

[R14] C 风格 for
来源：http://jjo.pengpengdd.cyou

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bje.ydjk.org.cn

[R15] while 逐行读文件
来源：http://lru.sjlbkw.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ifw.epnwcf.com

[R16] until 等待条件
来源：http://dxh.hfpthk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qmf.ybcxt.top

[R17] 数组定义与取值
来源：http://fxk.iojbl.cn

arr=(a b c); echo "${arr[0]}"
来源：http://liy.jiagoushi.top

[R18] 遍历数组
来源：http://cbb.sxryk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cvk.fehbvm.com

[R19] 数组长度
来源：http://yfc.hnxiangtu.top

echo "${#arr[@]}"
来源：http://fys.hnqzz.top

[R20] 关联数组（字典）
来源：http://dsh.jinghuilouyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gfk.pengpengdd.cyou

[R21] 字符串长度
来源：http://rjp.feifeiyinyue.top

echo "${#s}"
来源：http://gjy.ydjk.org.cn

[R22] 截取子串
来源：http://ick.tian-w.cn

echo "${s:0:5}"
来源：http://guu.svipenyu.cn

[R23] 字符串替换
来源：http://mrw.sweek.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xai.chenjidiqi.icu

[R24] 大小写转换
来源：http://yec.cashguo.top

echo "${s^^}"; echo "${s,,}"
来源：http://vub.c1oappe.top

[R25] 去后缀 / 去前缀
来源：http://zmq.hysaishi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gwl.snrcjt.cn

[R26] 命令替换
来源：http://ntf.zhengqikj.top

now=$(date +%F); echo "$now"
来源：http://ehh.yj202588.top

[R27] 算术展开
来源：http://ugv.fehbvm.com

echo $((1 + 2 * 3))
来源：http://sdk.sjlbkw.cn

[R28] 浮点运算
来源：http://cup.9152youxi.cn

echo "scale=2; 10/3" | bc
来源：http://hhv.feifeiyinyue.top

[R29] 定义函数
来源：http://hdh.jinqigfzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pbw.hnxiangtu.top

[R30] 函数返回状态码
来源：http://xzr.gzhubu.top

f() { return 0; }; f || echo "失败了"
来源：http://bjm.dashuyun.cn

[R31] 局部变量
来源：http://xma.yuxming.cn

f() { local x=1; echo "$x"; }
来源：http://uat.sweek.top

[R32] 参数个数校验
来源：http://bdp.epnwcf.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rep.pengpengdd.cyou

[R33] 捕获错误并提示行号
来源：http://zuj.haohaochexian.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tzb.zhoulong.xyz

[R34] 退出时清理
来源：http://gzr.haohaochexian.top

trap 'rm -f "$tmp"' EXIT
来源：http://mjg.yj20258888.top

[R35] 后台执行并等待
来源：http://ots.zhaomingkeji.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://cuz.feifeiyinyue.top

[R36] 并发执行多个任务
来源：http://tkr.vehdjk.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mwf.havefunace.top

[R37] 把输出赋给变量
来源：http://dvz.yj202588.top

files=$(ls -1)
来源：http://erp.hongshengwenyu.top

[R38] 管道串联
来源：http://uss.smart0.xyz

cat a.txt | grep -i error | wc -l
来源：http://dxx.zhaomingkeji.xyz

[R39] 重定向标准输出与错误
来源：http://jse.havefunace.top

cmd > out.log 2>&1
来源：http://oou.yvedp.cn

[R40] 追加写日志
来源：http://wva.cashguo.top

echo "log" >> out.log
来源：http://por.jlsjyb.cn

[R41] 丢弃输出
来源：http://umn.shangyingyoupin.top

cmd >/dev/null 2>&1
来源：http://sjw.ybcxt.top

[R42] 输入重定向
来源：http://jhu.yonumen.top

wc -l < a.txt
来源：http://pqe.ywan-chungtsiang.top

[R43] 按名字查找文件
来源：http://sdk.daxiang520.top

find . -name "*.log" -type f
来源：http://hjh.zhongyouzk.top

[R44] 按修改时间查找
来源：http://rtd.sufxvd.cn

find . -mtime -7 -type f
来源：http://rzk.nanxuanxn.top

[R45] 批量删除
来源：http://xlq.chenzaomai.com

find . -name "*.tmp" -delete
来源：http://hnn.jinqigfzy.top

[R46] 递归替换文件内容
来源：http://edp.yuxming.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yvc.haohaochexian.top

[R47] sed 单行替换
来源：http://tyb.ppjwa.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hkv.feifeiyinyue.top

[R48] awk 取指定列
来源：http://xwv.mhx1999.top

awk '{print $1, $3}' a.txt
来源：http://qne.zhixingplan.top

[R49] awk 带条件
来源：http://dep.quarkkingdee.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bdq.hesvh.cn

[R50] awk 求和
来源：http://ztv.hesvh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zpz.svipenyu.cn

[R51] 排序去重取前几
来源：http://soi.zycfv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bxn.zhiwuduotai.top

[R52] 统计行数
来源：http://nbb.ctjpmb.com

wc -l a.txt
来源：http://yog.hongshengwenyu.top

[R53] 查看文件头与实时尾
来源：http://hbp.bjfxy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jrl.yangfankeji.com

[R54] 比较两个文件
来源：http://pcb.zhoulong.xyz

diff a.txt b.txt
来源：http://gfa.fengsongda.top

[R55] 压缩与解压
来源：http://xuj.zycfv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yat.nanxinkj.top

[R56] 远程拷贝
来源：http://vuf.uphjek.com

scp file user@host:/path/
来源：http://fdg.mhx1999.top

[R57] 远程执行命令
来源：http://her.shzxlz.cn

ssh user@host 'uptime'
来源：http://pnn.zhongyouzk.top

[R58] 下载文件
来源：http://vxe.xinyue.icu

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oca.feifeiyinyue.top

[R59] 发 POST JSON
来源：http://rhs.shangyingyoupin.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xgv.hesvh.cn

[R60] 只看 HTTP 状态码
来源：http://utk.xziqi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kse.fzhhl.top

[R61] 磁盘占用
来源：http://idf.fengsongda.top

df -h;  du -sh *
来源：http://mqb.cdnleiting.top

[R62] 找最占空间的文件
来源：http://tit.guannengcc.top

du -ah . | sort -rh | head -10
来源：http://bdc.mhx1999.top

[R63] 内存与进程
来源：http://ptb.nwbrower.top

free -h;  ps aux | grep nginx
来源：http://nix.hfpthk.cn

[R64] 结束进程
来源：http://jhc.zhixingplan.top

kill -9 $(pgrep -f app.py)
来源：http://lgy.ivvv.top

[R65] 查看端口占用
来源：http://dbz.jiagoushi.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wer.uphjek.com

[R66] 定时任务
来源：http://gju.jlsjyb.cn

crontab -e;  crontab -l
来源：http://ilj.nwbrower.top

[R67] 生成随机十六进制串
来源：http://hiz.316326.xyz

openssl rand -hex 16
来源：http://csz.xylfe.cn

[R68] 计算文件校验值
来源：http://uwk.c1oappe.top

sha256sum a.txt;  md5sum a.txt
来源：http://smg.zhengqikj.top

[R69] 生成随机密码
来源：http://pjy.fehbvm.com

head -c 16 /dev/urandom | base64
来源：http://psx.bbcook.cn

[R70] 时间戳与互转
来源：http://nlt.ywan-chungtsiang.top

date +%s;  date -d @1700000000
来源：http://jdf.jinyuanbaomall.cn

[R71] 日期格式化
来源：http://bxx.zhengqikj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ccm.zdqjudy.top

[R72] 等待端口就绪
来源：http://exm.dashuyun.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://eqe.kuanghao11.cn

[R73] 分割大日志
来源：http://luo.yonumen.top

split -l 1000 big.log part_
来源：http://xnv.yj20258.top

[R74] 批量重命名
来源：http://rdv.guowangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ibx.havefunace.top

[R75] 导出环境变量
来源：http://jsr.zhoulong.xyz

export PATH="$HOME/bin:$PATH"
来源：http://qys.nanxinkj.top

[R76] 使用临时文件
来源：http://dvq.dianchejie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vxy.vehdjk.com

[R77] 读取用户输入
来源：http://pxz.cashguo.top

read -rp "请输入: " ans
来源：http://qnl.xinyue.icu

[R78] 交互式菜单
来源：http://gaz.vqdsnc.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rgy.cdnleiting.top

[R79] 解析命令行选项
来源：http://ezi.yanxiufei.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uxw.yfazqb.com

[R80] 查看脚本执行耗时
来源：http://cuz.hesvh.cn

time ./run.sh
来源：http://obw.zdbjq.cn

================================================================================
来源：http://bjn.tarul.cn

S. C / C++ 专题
来源：http://yrl.c1oappe.top

================================================================================
来源：http://yoa.zhixingplan.top

[S01] C：Hello World
来源：http://qij.iojbl.cn

#include <stdio.h>
来源：http://vdb.yuxming.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lwt.yonumen.top

[S02] C：变量与格式化输出
来源：http://ain.iojbl.cn

int a = 10; printf("%d\n", a);
来源：http://cmi.kuanghao11.cn

[S03] C：读入整数
来源：http://eqt.yj202588.top

int x; scanf("%d", &x);
来源：http://osb.guannengcc.top

[S04] C：字符串复制
来源：http://lip.bbcook.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lpj.ydzc1.top

[S05] C：字符串长度
来源：http://uok.redwolf501.top

strlen(s)
来源：http://igf.yfazqb.com

[S06] C：字符串比较
来源：http://xbq.sjlbkw.cn

strcmp(a, b) == 0
来源：http://eas.aibaodan.cn

[S07] C：数组遍历求和
来源：http://ngx.zdbjq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ttq.redwolf501.top

[S08] C：动态内存分配与释放
来源：http://swe.yj202588.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wyb.cqqwz.cn

[S09] C：结构体定义与初始化
来源：http://orj.hesvh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mai.zhongyouzk.top

[S10] C：指针与解引用
来源：http://imh.mhx1999.top

int *p = &a;  *p = 5;
来源：http://elp.ehwqpu.com

[S11] C：逐行读文件
来源：http://bpi.hywenlv.cn

FILE *f = fopen("a.txt", "r");
来源：http://yhd.hnqzz.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://syk.ybcxt.top

fclose(f);
来源：http://kvc.hammf.cn

[S12] C：写文件
来源：http://wrv.epnwcf.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rcu.zhiwuduotai.top

[S13] C：宏定义
来源：http://whh.yj202588.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yjd.gogol.net.cn

[S14] C：枚举
来源：http://lbx.yanxiufei.cn

enum Color { RED, GREEN, BLUE };
来源：http://ewq.feifeiyinyue.top

[S15] C：类型转换
来源：http://lbb.cheryme.top

(double) a / b
来源：http://rli.guannengcc.top

[S16] C：位操作置位
来源：http://dxq.fehbvm.com

x |= (1 << 3);
来源：http://iil.jinqigufen.top

[S17] C：安全拼接字符串
来源：http://obs.aizwys.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ueh.fzhhl.top

[S18] C：命令行参数
来源：http://his.fehbvm.com

int main(int argc, char **argv)
来源：http://eex.nanxuanxn.top

[S19] C：快速排序
来源：http://dcv.meibo888.top

qsort(a, n, sizeof(int), cmp);
来源：http://hlu.ywan-chungtsiang.top

[S20] C：二分查找
来源：http://lru.yonumen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rqb.zycfv.cn

[S21] C：字符类别判断
来源：http://kwg.hcnkem.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ceb.jqgufenzy.top

[S22] C：字符串转数字
来源：http://xpd.yongpay.top

atoi("42");  strtod("3.14", NULL);
来源：http://bng.hammf.cn

[S23] C：随机数
来源：http://eci.cqqwz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://crh.gaohongyu789.top

[S24] C：获取本地时间
来源：http://eqf.hnxiangtu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://twq.aibaodan.cn

[S25] C：内存拷贝
来源：http://qqo.ehwqpu.com

memcpy(dst, src, n);
来源：http://rdb.iojbl.cn

[S26] C：内存清零
来源：http://rsr.jqgufenzy.top

memset(a, 0, sizeof a);
来源：http://gap.fktsv.cn

[S27] C：定义常量
来源：http://dbi.nwbrower.top

const double PI = 3.14159;
来源：http://vnn.pengpengdd.cyou

[S28] C：静态变量
来源：http://nyi.zhiwuduotai.top

static int counter = 0;
来源：http://kcd.hywenlv.cn

[S29] C：变参函数
来源：http://trg.pycfn.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wmn.sweek.top

[S30] C：头文件保护
来源：http://byp.xuetiantiany.cn

#ifndef X_H
来源：http://wnp.chenzaomai.com

#define X_H
来源：http://pqp.smart0.xyz

#endif
来源：http://sxa.yongpay.top

[S31] C++：Hello World
来源：http://edk.zhaomingkeji.xyz

#include <iostream>
来源：http://oxo.wangdashe.top

int main() { std::cout << "Hello\n"; }
来源：http://tdn.jqgfzy.top

[S32] C++：字符串
来源：http://spj.yuxming.cn

std::string s = "hi";  s += "!";
来源：http://zpe.quarkkingdee.top

[S33] C++：vector 增删
来源：http://kjj.hysaishi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hzd.shuidangran.top

[S34] C++：遍历 vector
来源：http://vdc.vehdjk.com

for (auto &x : v) { std::cout << x; }
来源：http://oxp.52xcode.cn

[S35] C++：map
来源：http://mkq.xuetiantiany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vks.zhengqikj.top

[S36] C++：unordered_map
来源：http://fqr.hywenlv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://osb.yanxiufei.cn

[S37] C++：set
来源：http://pmb.hongshengwenyu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kje.xylfe.cn

[S38] C++：排序
来源：http://mjt.cdnleiting.top

std::sort(v.begin(), v.end());
来源：http://mzn.jinghuilouyu.cn

[S39] C++：自定义比较器排序
来源：http://ujd.meibo888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ura.zhaomingkeji.xyz

[S40] C++：查找元素
来源：http://eik.ydzc1.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ods.tian-w.cn

[S41] C++：类与构造函数
来源：http://kwn.feifeiyinyue.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pvu.daxiang520.top

[S42] C++：继承与虚函数
来源：http://eym.yongpay.top

class B : public Base { public: void f() override {} };
来源：http://ioy.yongpay.top

[S43] C++：智能指针
来源：http://zhp.nanxinkj.top

auto p = std::make_unique<int>(5);
来源：http://oql.jlsjyb.cn

[S44] C++：引用传参
来源：http://xvr.cucudq.cn

void inc(int &x) { ++x; }
来源：http://gou.sweek.top

[S45] C++：lambda
来源：http://cck.yueranfly.top

auto add = [](int a, int b) { return a + b; };
来源：http://sty.jinqigufen.top

[S46] C++：函数模板
来源：http://fws.ivvv.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qnv.hnxiangtu.top

[S47] C++：结构化绑定遍历
来源：http://wxy.guannengcc.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cny.andypj.xyz

[S48] C++：逐行读文件
来源：http://mit.fehbvm.com

std::ifstream in("a.txt");  std::string line;
来源：http://irt.fktsv.cn

while (std::getline(in, line)) { }
来源：http://zqx.cucudq.cn

[S49] C++：写文件
来源：http://yjd.yfazqb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qfs.yvedp.cn

[S50] C++：格式化数字
来源：http://ock.yongpay.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mpc.fktsv.cn

[S51] C++：显式类型转换
来源：http://rnd.yueranfly.top

static_cast<double>(a) / b
来源：http://ffo.tanke756.top

[S52] C++：const 与 noexcept
来源：http://hvj.yj20258888.top

int size() const noexcept { return n_; }
来源：http://fwd.hesvh.cn

[S53] C++：移动语义
来源：http://szp.xingfuxueyuan.xyz

std::vector<int> w = std::move(v);
来源：http://cro.smart0.xyz

[S54] C++：异常处理
来源：http://mbr.zdbjq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mbj.yj202588.top

[S55] C++：结构化绑定
来源：http://frk.zhijiandao.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rsk.jqgfzy.top

[S56] C++：optional
来源：http://cwp.yvedp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mzx.zhixingplan.top

[S57] C++：编译期常量
来源：http://yps.wangdashe.top

constexpr int N = 10;
来源：http://eqt.zhongyouzk.top

[S58] C++：命名空间
来源：http://wps.316326.xyz

namespace ns { int f() { return 1; } }
来源：http://arz.birdmap.top

[S59] C++：静态断言
来源：http://pfz.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wfl.jlsjyb.cn

[S60] C++：遍历并删除元素
来源：http://zon.snrcjt.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://odi.mhx1999.top

================================================================================
来源：http://ggu.chenjidiqi.icu

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dnb.guannengcc.top

================================================================================
来源：http://vey.jianghu66.top

[T01] Kotlin：Hello World
来源：http://fjp.sxryk.cn

println("Hello")
来源：http://viv.hesvh.cn

[T02] Kotlin：变量
来源：http://efj.kuanghao11.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rjl.nwbrower.top

[T03] Kotlin：字符串模板
来源：http://oka.aibaodan.cn

"值: $b"
来源：http://gde.zhixingplan.top

[T04] Kotlin：空安全
来源：http://hix.aizwys.cn

val n: String? = null;  n?.length
来源：http://mlq.zdbjq.cn

[T05] Kotlin：when 表达式
来源：http://uxo.fktsv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://drw.jlsjyb.cn

[T06] Kotlin：集合映射
来源：http://cwy.jinyuanbaomall.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cqc.snrcjt.cn

[T07] Kotlin：集合过滤
来源：http://ycd.sysykeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rud.jinghuilouyu.cn

[T08] Kotlin：数据类
来源：http://lll.xingfuxueyuan.xyz

data class User(val name: String, val age: Int)
来源：http://ebi.jinqigfzy.top

[T09] Kotlin：扩展函数
来源：http://bty.yonumen.top

fun String.exclaim() = this + "!"
来源：http://gad.yj20258888.top

[T10] Kotlin：默认参数
来源：http://mto.tarul.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://njl.cashguo.top


<!-- 参考信息 -->