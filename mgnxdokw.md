代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://utu.tianlin.xyz

[R10] 正则匹配
来源：http://zqw.ppjwa.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://aff.ivvv.top

[R11] case 多分支
来源：http://eoz.sufxvd.cn

case "$1" in
来源：http://dyx.zhongyouzk.top

start) echo "启动" ;;
来源：http://cde.sjlbkw.cn

stop)  echo "停止" ;;
来源：http://jea.gzhubu.top

*)     echo "未知命令" ;;
来源：http://gax.svipenyu.cn

esac
来源：http://ntr.jinqigfzy.top

[R12] for 遍历文件
来源：http://giu.dashuyun.cn

for f in *.txt; do echo "$f"; done
来源：http://lgx.bjfxy.top

[R13] for 计数循环
来源：http://fjg.wangshuangyany.cn

for i in {1..10}; do echo "$i"; done
来源：http://rfc.zdbjq.cn

[R14] C 风格 for
来源：http://zpb.fengsongda.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mbd.meibo888.top

[R15] while 逐行读文件
来源：http://zpd.jqgufenzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yiy.andypj.xyz

[R16] until 等待条件
来源：http://egw.xuetiantiany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xyv.gogol.net.cn

[R17] 数组定义与取值
来源：http://ryb.uphjek.com

arr=(a b c); echo "${arr[0]}"
来源：http://rrq.hysaishi.cn

[R18] 遍历数组
来源：http://iwf.cqqwz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yrc.yuxming.cn

[R19] 数组长度
来源：http://zmf.zhixingplan.top

echo "${#arr[@]}"
来源：http://nao.aizwys.cn

[R20] 关联数组（字典）
来源：http://zoq.tanke756.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zoa.smart0.xyz

[R21] 字符串长度
来源：http://lnk.tian-w.cn

echo "${#s}"
来源：http://ppr.hongshengwenyu.top

[R22] 截取子串
来源：http://yxz.ctjpmb.com

echo "${s:0:5}"
来源：http://jsb.ybcxt.top

[R23] 字符串替换
来源：http://ewp.pycfn.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yob.vehdjk.com

[R24] 大小写转换
来源：http://wpp.andypj.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://ezp.yueranfly.top

[R25] 去后缀 / 去前缀
来源：http://twv.pengpengdd.cyou

echo "${f%.txt}"; echo "${f#./}"
来源：http://saq.tian-w.cn

[R26] 命令替换
来源：http://ovk.kuanghao11.cn

now=$(date +%F); echo "$now"
来源：http://fzn.hnxiangtu.top

[R27] 算术展开
来源：http://nfm.vehdjk.com

echo $((1 + 2 * 3))
来源：http://zkb.ywan-chungtsiang.top

[R28] 浮点运算
来源：http://hqy.meibo888.top

echo "scale=2; 10/3" | bc
来源：http://hkv.shanyushiyangkeji.top

[R29] 定义函数
来源：http://acx.ydjk.org.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ssn.epnwcf.com

[R30] 函数返回状态码
来源：http://ixp.fanxiaobao.xyz

f() { return 0; }; f || echo "失败了"
来源：http://tdy.xingfuxueyuan.xyz

[R31] 局部变量
来源：http://knb.yj202588.top

f() { local x=1; echo "$x"; }
来源：http://szz.fzhhl.top

[R32] 参数个数校验
来源：http://hdb.52xcode.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jof.snrcjt.cn

[R33] 捕获错误并提示行号
来源：http://byy.hnxiangtu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rdx.ctjpmb.com

[R34] 退出时清理
来源：http://bmy.zdbjq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://eqm.xuanzx.com

[R35] 后台执行并等待
来源：http://pim.haohaochexian.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wkv.xziqi.cn

[R36] 并发执行多个任务
来源：http://sid.0kj1m.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cde.jinqigfzy.top

[R37] 把输出赋给变量
来源：http://rsf.xylfe.cn

files=$(ls -1)
来源：http://zmh.jianghu66.top

[R38] 管道串联
来源：http://nfj.zhijiandao.cn

cat a.txt | grep -i error | wc -l
来源：http://evb.smart0.xyz

[R39] 重定向标准输出与错误
来源：http://ipg.chenjidiqi.icu

cmd > out.log 2>&1
来源：http://erg.havefunace.top

[R40] 追加写日志
来源：http://yui.yuanzhike.top

echo "log" >> out.log
来源：http://kbj.316326.xyz

[R41] 丢弃输出
来源：http://dkr.guannengcc.top

cmd >/dev/null 2>&1
来源：http://cpi.yonumen.top

[R42] 输入重定向
来源：http://kht.havefunace.top

wc -l < a.txt
来源：http://bko.gzhubu.top

[R43] 按名字查找文件
来源：http://frc.xuetiantiany.cn

find . -name "*.log" -type f
来源：http://ygv.kuanghao11.cn

[R44] 按修改时间查找
来源：http://hup.chenjidiqi.icu

find . -mtime -7 -type f
来源：http://hoq.pengpengdd.cyou

[R45] 批量删除
来源：http://qpe.jlsjyb.cn

find . -name "*.tmp" -delete
来源：http://hjd.jinqigufen.top

[R46] 递归替换文件内容
来源：http://hdy.yj202588.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mbd.redwolf501.top

[R47] sed 单行替换
来源：http://rze.jinghuilouyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fnl.tarul.cn

[R48] awk 取指定列
来源：http://zzy.zhixingplan.top

awk '{print $1, $3}' a.txt
来源：http://oki.xylfe.cn

[R49] awk 带条件
来源：http://uvo.wangshuangyany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cuk.xuanzx.com

[R50] awk 求和
来源：http://zlu.xuanzx.com

awk '{s += $2} END {print s}' a.txt
来源：http://fxu.feifeiyinyue.top

[R51] 排序去重取前几
来源：http://spv.316326.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://opi.shuidangran.top

[R52] 统计行数
来源：http://ozt.wangshuangyany.cn

wc -l a.txt
来源：http://ipv.haohaochexian.top

[R53] 查看文件头与实时尾
来源：http://idf.yongpay.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wkp.316326.xyz

[R54] 比较两个文件
来源：http://uyq.svipenyu.cn

diff a.txt b.txt
来源：http://gts.jlsjyb.cn

[R55] 压缩与解压
来源：http://ube.cdnleiting.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yge.andypj.xyz

[R56] 远程拷贝
来源：http://izv.yj20258.top

scp file user@host:/path/
来源：http://gsp.xziqi.cn

[R57] 远程执行命令
来源：http://vjr.gaohongyu789.top

ssh user@host 'uptime'
来源：http://glh.sxryk.cn

[R58] 下载文件
来源：http://aab.hcnkem.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gmr.redwolf501.top

[R59] 发 POST JSON
来源：http://gny.zycfv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vfh.9152youxi.cn

[R60] 只看 HTTP 状态码
来源：http://wte.shzxlz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gkz.vehdjk.com

[R61] 磁盘占用
来源：http://gew.vqdsnc.cn

df -h;  du -sh *
来源：http://uoi.svipenyu.cn

[R62] 找最占空间的文件
来源：http://olm.yj20258.top

du -ah . | sort -rh | head -10
来源：http://xeg.chenlongwang.top

[R63] 内存与进程
来源：http://hhh.wangshuangyany.cn

free -h;  ps aux | grep nginx
来源：http://jvf.chenzaomai.com

[R64] 结束进程
来源：http://egx.jinghuilouyu.cn

kill -9 $(pgrep -f app.py)
来源：http://wee.svipenyu.cn

[R65] 查看端口占用
来源：http://duq.ydjk.org.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://itm.meibo888.top

[R66] 定时任务
来源：http://dcf.316326.xyz

crontab -e;  crontab -l
来源：http://uwg.svipenyu.cn

[R67] 生成随机十六进制串
来源：http://oxl.hcnkem.com

openssl rand -hex 16
来源：http://nrf.yj20258888.top

[R68] 计算文件校验值
来源：http://xsw.haohaochexian.top

sha256sum a.txt;  md5sum a.txt
来源：http://qon.daria6918.cn

[R69] 生成随机密码
来源：http://zyz.cqqwz.cn

head -c 16 /dev/urandom | base64
来源：http://ujv.gotoacloud.top

[R70] 时间戳与互转
来源：http://mxt.hesvh.cn

date +%s;  date -d @1700000000
来源：http://vju.hesvh.cn

[R71] 日期格式化
来源：http://cxq.nanxinkj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://fpz.yuxming.cn

[R72] 等待端口就绪
来源：http://rel.yj202588.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wei.dashuyun.cn

[R73] 分割大日志
来源：http://dcx.nanxinkj.top

split -l 1000 big.log part_
来源：http://fay.quarkkingdee.top

[R74] 批量重命名
来源：http://aky.havefunace.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sje.haohaochexian.top

[R75] 导出环境变量
来源：http://sos.ehwqpu.com

export PATH="$HOME/bin:$PATH"
来源：http://kxv.jinqigufen.top

[R76] 使用临时文件
来源：http://cqd.wangdashe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fam.svipenyu.cn

[R77] 读取用户输入
来源：http://wbl.dianchejie.cn

read -rp "请输入: " ans
来源：http://qvt.gzhubu.top

[R78] 交互式菜单
来源：http://ghh.dianchejie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tts.zhijiandao.cn

[R79] 解析命令行选项
来源：http://zwj.xziqi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lan.zhaomingkeji.xyz

[R80] 查看脚本执行耗时
来源：http://nvh.fzhhl.top

time ./run.sh
来源：http://ncc.yanxiufei.cn

================================================================================
来源：http://lmq.hcnkem.com

S. C / C++ 专题
来源：http://emr.ybcxt.top

================================================================================
来源：http://phg.yongpay.top

[S01] C：Hello World
来源：http://fge.hnqzz.top

#include <stdio.h>
来源：http://rws.jlsjyb.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ggf.haohaochexian.top

[S02] C：变量与格式化输出
来源：http://qzn.hesvh.cn

int a = 10; printf("%d\n", a);
来源：http://ufo.wangshuangyany.cn

[S03] C：读入整数
来源：http://ezl.cucudq.cn

int x; scanf("%d", &x);
来源：http://omy.sjlbkw.cn

[S04] C：字符串复制
来源：http://igq.daxiang520.top

char dst[32]; strcpy(dst, "hi");
来源：http://tel.yj20258.top

[S05] C：字符串长度
来源：http://spr.yonumen.top

strlen(s)
来源：http://xou.chenjidiqi.icu

[S06] C：字符串比较
来源：http://irg.kuanghao11.cn

strcmp(a, b) == 0
来源：http://gsv.yuanzhike.top

[S07] C：数组遍历求和
来源：http://oze.chenzaomai.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oyi.hywenlv.cn

[S08] C：动态内存分配与释放
来源：http://gij.yonumen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://myo.fzhhl.top

[S09] C：结构体定义与初始化
来源：http://gas.jianghu66.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dmo.bbcook.cn

[S10] C：指针与解引用
来源：http://tzd.hnqzz.top

int *p = &a;  *p = 5;
来源：http://smc.vehdjk.com

[S11] C：逐行读文件
来源：http://nmi.andypj.xyz

FILE *f = fopen("a.txt", "r");
来源：http://pjt.yanxiufei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wnp.vqdsnc.cn

fclose(f);
来源：http://bxw.redwolf501.top

[S12] C：写文件
来源：http://hzd.nanxuanxn.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://udd.uphjek.com

[S13] C：宏定义
来源：http://xrd.snrcjt.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://etv.zhijiandao.cn

[S14] C：枚举
来源：http://tkd.fktsv.cn

enum Color { RED, GREEN, BLUE };
来源：http://blc.zhoulong.xyz

[S15] C：类型转换
来源：http://rxf.zycfv.cn

(double) a / b
来源：http://qrl.guannengcc.top

[S16] C：位操作置位
来源：http://fmu.9152youxi.cn

x |= (1 << 3);
来源：http://lhc.xingfuxueyuan.xyz

[S17] C：安全拼接字符串
来源：http://dfn.yongpay.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ddm.zhongyouzk.top

[S18] C：命令行参数
来源：http://shz.cucudq.cn

int main(int argc, char **argv)
来源：http://tat.meibo888.top

[S19] C：快速排序
来源：http://ajc.jinqigufen.top

qsort(a, n, sizeof(int), cmp);
来源：http://wqj.havefunace.top

[S20] C：二分查找
来源：http://rfl.tianlin.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://djv.xziqi.cn

[S21] C：字符类别判断
来源：http://xvk.nwbrower.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://idf.zycfv.cn

[S22] C：字符串转数字
来源：http://whq.uphjek.com

atoi("42");  strtod("3.14", NULL);
来源：http://qba.chenzaomai.com

[S23] C：随机数
来源：http://wqt.xziqi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://awq.yj20258888.top

[S24] C：获取本地时间
来源：http://cdq.sysykeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://omb.52xcode.cn

[S25] C：内存拷贝
来源：http://lop.fengsongda.top

memcpy(dst, src, n);
来源：http://ojj.bbcook.cn

[S26] C：内存清零
来源：http://jdq.jinghuilouyu.cn

memset(a, 0, sizeof a);
来源：http://khp.pycfn.com

[S27] C：定义常量
来源：http://vka.bbcook.cn

const double PI = 3.14159;
来源：http://uoh.vehdjk.com

[S28] C：静态变量
来源：http://uny.jinqigufen.top

static int counter = 0;
来源：http://ocx.dianchejie.cn

[S29] C：变参函数
来源：http://bgk.fktsv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ymk.zhongyouzk.top

[S30] C：头文件保护
来源：http://cqr.zycfv.cn

#ifndef X_H
来源：http://xhn.vqdsnc.cn

#define X_H
来源：http://oxf.gogol.net.cn

#endif
来源：http://xbf.mhx1999.top

[S31] C++：Hello World
来源：http://sou.0kj1m.cn

#include <iostream>
来源：http://vjo.feifeiyinyue.top

int main() { std::cout << "Hello\n"; }
来源：http://oit.zdbjq.cn

[S32] C++：字符串
来源：http://vfk.redwolf501.top

std::string s = "hi";  s += "!";
来源：http://try.cdnleiting.top

[S33] C++：vector 增删
来源：http://ghc.kuanghao11.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kvo.ydzc1.top

[S34] C++：遍历 vector
来源：http://rxy.xuanzx.com

for (auto &x : v) { std::cout << x; }
来源：http://xzl.kuanghao11.cn

[S35] C++：map
来源：http://waa.zycfv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ajx.cqqwz.cn

[S36] C++：unordered_map
来源：http://jls.mhx1999.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eqx.chenjidiqi.icu

[S37] C++：set
来源：http://qxa.xingfuxueyuan.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bas.jianghu66.top

[S38] C++：排序
来源：http://rdd.yj20258888.top

std::sort(v.begin(), v.end());
来源：http://ztg.zdqjudy.top

[S39] C++：自定义比较器排序
来源：http://bek.shuidangran.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qsf.ivvv.top

[S40] C++：查找元素
来源：http://ban.zhoulong.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kzn.smart0.xyz

[S41] C++：类与构造函数
来源：http://qpx.fzhhl.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://svh.bbcook.cn

[S42] C++：继承与虚函数
来源：http://fja.zhaomingkeji.xyz

class B : public Base { public: void f() override {} };
来源：http://wkt.hongshengwenyu.top

[S43] C++：智能指针
来源：http://set.zhixingplan.top

auto p = std::make_unique<int>(5);
来源：http://haj.yj20258.top

[S44] C++：引用传参
来源：http://iao.9152youxi.cn

void inc(int &x) { ++x; }
来源：http://cat.shzxlz.cn

[S45] C++：lambda
来源：http://xor.iojbl.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bvl.pycfn.com

[S46] C++：函数模板
来源：http://lyj.ywan-chungtsiang.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uge.yanxiufei.cn

[S47] C++：结构化绑定遍历
来源：http://tvt.aizwys.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jdt.jianghu66.top

[S48] C++：逐行读文件
来源：http://yyo.ywan-chungtsiang.top

std::ifstream in("a.txt");  std::string line;
来源：http://sde.chenjidiqi.icu

while (std::getline(in, line)) { }
来源：http://ife.gzhubu.top

[S49] C++：写文件
来源：http://gab.tarul.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hzr.hnqzz.top

[S50] C++：格式化数字
来源：http://awl.yongpay.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tab.52xcode.cn

[S51] C++：显式类型转换
来源：http://hbe.nanxinkj.top

static_cast<double>(a) / b
来源：http://omx.kuanghao11.cn

[S52] C++：const 与 noexcept
来源：http://cyt.pengpengdd.cyou

int size() const noexcept { return n_; }
来源：http://rol.chenjidiqi.icu

[S53] C++：移动语义
来源：http://cce.pycfn.com

std::vector<int> w = std::move(v);
来源：http://pye.fktsv.cn

[S54] C++：异常处理
来源：http://akw.aibaodan.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://aah.ctjpmb.com

[S55] C++：结构化绑定
来源：http://jtt.tianlin.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://cbq.aizwys.cn

[S56] C++：optional
来源：http://uud.yfazqb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://orx.kuanghao11.cn

[S57] C++：编译期常量
来源：http://liy.bbcook.cn

constexpr int N = 10;
来源：http://hci.iojbl.cn

[S58] C++：命名空间
来源：http://mlc.jqgufenzy.top

namespace ns { int f() { return 1; } }
来源：http://obu.haohaochexian.top

[S59] C++：静态断言
来源：http://bha.havefunace.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ham.xinyue.icu

[S60] C++：遍历并删除元素
来源：http://rfv.fanxiaobao.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://feh.tanke756.top

================================================================================
来源：http://guu.shanyushiyangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jdd.jiagoushi.top

================================================================================
来源：http://gge.gzhubu.top

[T01] Kotlin：Hello World
来源：http://nwu.tanke756.top

println("Hello")
来源：http://tfm.xziqi.cn

[T02] Kotlin：变量
来源：http://pku.jinqigufen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vxv.chenlongwang.top

[T03] Kotlin：字符串模板
来源：http://zgd.ehwqpu.com

"值: $b"
来源：http://zzj.redwolf501.top

[T04] Kotlin：空安全
来源：http://uoh.shzxlz.cn

val n: String? = null;  n?.length
来源：http://erm.cucudq.cn

[T05] Kotlin：when 表达式
来源：http://gvo.zhongyouzk.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ngg.sweek.top

[T06] Kotlin：集合映射
来源：http://xxq.zhoulong.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://xkp.fktsv.cn

[T07] Kotlin：集合过滤
来源：http://wms.tianlin.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://qss.gogol.net.cn

[T08] Kotlin：数据类
来源：http://pud.nwbrower.top

data class User(val name: String, val age: Int)
来源：http://ely.meibo888.top

[T09] Kotlin：扩展函数
来源：http://qns.yonumen.top

fun String.exclaim() = this + "!"
来源：http://veg.shanyushiyangtech.top

[T10] Kotlin：默认参数
来源：http://oud.yj20258888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://slb.uphjek.com


<!-- 参考信息 -->