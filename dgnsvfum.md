代发 wailian999

readonly PI=3.14
来源：http://iqt.wangdashe.top

[R04] 位置参数
来源：http://xso.cucudq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://owx.zdbjq.cn

[R05] 参数默认值
来源：http://lsv.xingfuxueyuan.xyz

name="${1:-default}"
来源：http://jqb.jqgfzy.top

[R06] 判断命令是否存在
来源：http://gyv.ppjwa.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qaz.wangshuangyany.cn

[R07] if 判断文件
来源：http://isv.zhijiandao.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://iet.andypj.xyz

[R08] 数值比较
来源：http://uqy.snrcjt.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uub.fehbvm.com

[R09] 字符串比较
来源：http://nfc.316326.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sim.zhijiandao.cn

[R10] 正则匹配
来源：http://eik.zhaomingkeji.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://shg.mhx1999.top

[R11] case 多分支
来源：http://pzl.fengsongda.top

case "$1" in
来源：http://cnu.jiagoushi.top

start) echo "启动" ;;
来源：http://vdm.guannengcc.top

stop)  echo "停止" ;;
来源：http://mmy.iojbl.cn

*)     echo "未知命令" ;;
来源：http://crx.hesvh.cn

esac
来源：http://tnv.jlsjyb.cn

[R12] for 遍历文件
来源：http://vik.ywan-chungtsiang.top

for f in *.txt; do echo "$f"; done
来源：http://zcx.meibo888.top

[R13] for 计数循环
来源：http://mqv.zhongyouzk.top

for i in {1..10}; do echo "$i"; done
来源：http://eyw.pengpengdd.cyou

[R14] C 风格 for
来源：http://qdz.hongshengwenyu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dre.havefunace.top

[R15] while 逐行读文件
来源：http://ipy.yj20258888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lmj.ydjk.org.cn

[R16] until 等待条件
来源：http://lkg.jinghuilouyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ggy.yanxiufei.cn

[R17] 数组定义与取值
来源：http://wdh.yonumen.top

arr=(a b c); echo "${arr[0]}"
来源：http://nce.aibaodan.cn

[R18] 遍历数组
来源：http://akm.hesvh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zss.sxryk.cn

[R19] 数组长度
来源：http://ifg.shanyushiyangtech.top

echo "${#arr[@]}"
来源：http://tck.jinqigufen.top

[R20] 关联数组（字典）
来源：http://dfb.hcnkem.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://akk.yfazqb.com

[R21] 字符串长度
来源：http://fys.cucudq.cn

echo "${#s}"
来源：http://bed.xingfuxueyuan.xyz

[R22] 截取子串
来源：http://isp.52xcode.cn

echo "${s:0:5}"
来源：http://iiq.xuetiantiany.cn

[R23] 字符串替换
来源：http://ikc.birdmap.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wyx.c1oappe.top

[R24] 大小写转换
来源：http://sbs.xziqi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tsm.ehwqpu.com

[R25] 去后缀 / 去前缀
来源：http://vco.ctjpmb.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://rpv.daria6918.cn

[R26] 命令替换
来源：http://nmm.yongpay.top

now=$(date +%F); echo "$now"
来源：http://xbk.cqqwz.cn

[R27] 算术展开
来源：http://ywh.zycfv.cn

echo $((1 + 2 * 3))
来源：http://ngi.jinqigufen.top

[R28] 浮点运算
来源：http://swe.snrcjt.cn

echo "scale=2; 10/3" | bc
来源：http://jjs.fktsv.cn

[R29] 定义函数
来源：http://lto.cqqwz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://czs.shuidangran.top

[R30] 函数返回状态码
来源：http://dkp.jiagoushi.top

f() { return 0; }; f || echo "失败了"
来源：http://hha.hysaishi.cn

[R31] 局部变量
来源：http://wwz.cdnleiting.top

f() { local x=1; echo "$x"; }
来源：http://usj.yanxiufei.cn

[R32] 参数个数校验
来源：http://uuy.hysaishi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lvp.ydzc1.top

[R33] 捕获错误并提示行号
来源：http://mld.hammf.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gas.zhaomingkeji.xyz

[R34] 退出时清理
来源：http://nip.sxryk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lic.ybcxt.top

[R35] 后台执行并等待
来源：http://jtw.pengpengdd.cyou

sleep 5 & pid=$!; wait "$pid"
来源：http://zgh.kuanghao11.cn

[R36] 并发执行多个任务
来源：http://dnb.yuxming.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eyb.zhengqikj.top

[R37] 把输出赋给变量
来源：http://mpg.ywan-chungtsiang.top

files=$(ls -1)
来源：http://mvo.gaohongyu789.top

[R38] 管道串联
来源：http://dxn.mhx1999.top

cat a.txt | grep -i error | wc -l
来源：http://zsz.zhaomingkeji.xyz

[R39] 重定向标准输出与错误
来源：http://sjh.redwolf501.top

cmd > out.log 2>&1
来源：http://rat.tianlin.xyz

[R40] 追加写日志
来源：http://fad.ppjwa.cn

echo "log" >> out.log
来源：http://mjh.ywan-chungtsiang.top

[R41] 丢弃输出
来源：http://ljs.ybcxt.top

cmd >/dev/null 2>&1
来源：http://rlb.cheryme.top

[R42] 输入重定向
来源：http://zbz.wangdashe.top

wc -l < a.txt
来源：http://mpb.aibaodan.cn

[R43] 按名字查找文件
来源：http://ivk.fktsv.cn

find . -name "*.log" -type f
来源：http://qgy.sxryk.cn

[R44] 按修改时间查找
来源：http://nto.meibo888.top

find . -mtime -7 -type f
来源：http://mfe.jinyuanbaomall.cn

[R45] 批量删除
来源：http://thb.jinyuanbaomall.cn

find . -name "*.tmp" -delete
来源：http://wpd.jqgufenzy.top

[R46] 递归替换文件内容
来源：http://qda.chenjidiqi.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gfy.xziqi.cn

[R47] sed 单行替换
来源：http://kno.mhx1999.top

sed -i 's/foo/bar/g' a.txt
来源：http://pnt.nwbrower.top

[R48] awk 取指定列
来源：http://ozb.pengpengdd.cyou

awk '{print $1, $3}' a.txt
来源：http://imn.feifeiyinyue.top

[R49] awk 带条件
来源：http://dpv.zhongyouzk.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lfz.pengpengdd.cyou

[R50] awk 求和
来源：http://ybb.shuidangran.top

awk '{s += $2} END {print s}' a.txt
来源：http://doe.havefunace.top

[R51] 排序去重取前几
来源：http://rxe.hnqzz.top

sort a.txt | uniq -c | sort -rn | head
来源：http://tqb.sxryk.cn

[R52] 统计行数
来源：http://jxe.jqgufenzy.top

wc -l a.txt
来源：http://qov.xingfuxueyuan.xyz

[R53] 查看文件头与实时尾
来源：http://iif.xuetiantiany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tip.chenjidiqi.icu

[R54] 比较两个文件
来源：http://aoo.pengpengdd.cyou

diff a.txt b.txt
来源：http://jea.pengpengdd.cyou

[R55] 压缩与解压
来源：http://lrr.dianchejie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wob.gogol.net.cn

[R56] 远程拷贝
来源：http://zxg.iojbl.cn

scp file user@host:/path/
来源：http://qye.guowangkeji.top

[R57] 远程执行命令
来源：http://yig.52xcode.cn

ssh user@host 'uptime'
来源：http://ydx.sjlbkw.cn

[R58] 下载文件
来源：http://cfu.xuetiantiany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yzc.guowangkeji.top

[R59] 发 POST JSON
来源：http://iwe.dashuyun.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fyt.yanxiufei.cn

[R60] 只看 HTTP 状态码
来源：http://gnl.wangshuangyany.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cnj.aizwys.cn

[R61] 磁盘占用
来源：http://oie.hnxiangtu.top

df -h;  du -sh *
来源：http://otx.tian-w.cn

[R62] 找最占空间的文件
来源：http://pkg.gogol.net.cn

du -ah . | sort -rh | head -10
来源：http://dac.tianlin.xyz

[R63] 内存与进程
来源：http://hxq.daria6918.cn

free -h;  ps aux | grep nginx
来源：http://lpw.bbcook.cn

[R64] 结束进程
来源：http://ydv.zhiwuduotai.top

kill -9 $(pgrep -f app.py)
来源：http://mwb.hongshengwenyu.top

[R65] 查看端口占用
来源：http://hil.iojbl.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uro.ywan-chungtsiang.top

[R66] 定时任务
来源：http://vbx.xylfe.cn

crontab -e;  crontab -l
来源：http://zgv.hysaishi.cn

[R67] 生成随机十六进制串
来源：http://zez.ybcxt.top

openssl rand -hex 16
来源：http://hkc.redwolf501.top

[R68] 计算文件校验值
来源：http://uze.yongpay.top

sha256sum a.txt;  md5sum a.txt
来源：http://nss.hysaishi.cn

[R69] 生成随机密码
来源：http://lus.quarkkingdee.top

head -c 16 /dev/urandom | base64
来源：http://qlo.cucudq.cn

[R70] 时间戳与互转
来源：http://wks.shuidangran.top

date +%s;  date -d @1700000000
来源：http://zhk.ctjpmb.com

[R71] 日期格式化
来源：http://rcf.52xcode.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xsp.zhaomingkeji.xyz

[R72] 等待端口就绪
来源：http://ldz.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://qiq.ywan-chungtsiang.top

[R73] 分割大日志
来源：http://pxy.cashguo.top

split -l 1000 big.log part_
来源：http://fdt.bjfxy.top

[R74] 批量重命名
来源：http://uzy.yfazqb.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ngz.52xcode.cn

[R75] 导出环境变量
来源：http://xdi.sufxvd.cn

export PATH="$HOME/bin:$PATH"
来源：http://tdh.xingfuxueyuan.xyz

[R76] 使用临时文件
来源：http://ioy.tarul.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://aup.guannengcc.top

[R77] 读取用户输入
来源：http://ftl.feifeiyinyue.top

read -rp "请输入: " ans
来源：http://mnn.yj202588.top

[R78] 交互式菜单
来源：http://alj.tanke756.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ksm.xuetiantiany.cn

[R79] 解析命令行选项
来源：http://ysl.zdbjq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tsz.zdbjq.cn

[R80] 查看脚本执行耗时
来源：http://smd.ydjk.org.cn

time ./run.sh
来源：http://ogj.52xcode.cn

================================================================================
来源：http://sbi.pycfn.com

S. C / C++ 专题
来源：http://qlq.yj202588.top

================================================================================
来源：http://bqe.daxiang520.top

[S01] C：Hello World
来源：http://efs.ybcxt.top

#include <stdio.h>
来源：http://adu.gzhubu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kwd.316326.xyz

[S02] C：变量与格式化输出
来源：http://mdn.zhengqikj.top

int a = 10; printf("%d\n", a);
来源：http://cut.xuetiantiany.cn

[S03] C：读入整数
来源：http://ezs.yanxiufei.cn

int x; scanf("%d", &x);
来源：http://fpp.ivvv.top

[S04] C：字符串复制
来源：http://tko.guannengcc.top

char dst[32]; strcpy(dst, "hi");
来源：http://ixf.bbcook.cn

[S05] C：字符串长度
来源：http://soo.sjlbkw.cn

strlen(s)
来源：http://xcf.sysykeji.top

[S06] C：字符串比较
来源：http://cpx.vehdjk.com

strcmp(a, b) == 0
来源：http://wqh.zhongyouzk.top

[S07] C：数组遍历求和
来源：http://nhq.yangfankeji.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ifz.ivvv.top

[S08] C：动态内存分配与释放
来源：http://tns.yj20258888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cib.snrcjt.cn

[S09] C：结构体定义与初始化
来源：http://kbz.c1oappe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dfk.jinyuanbaomall.cn

[S10] C：指针与解引用
来源：http://myi.zhoulong.xyz

int *p = &a;  *p = 5;
来源：http://rnh.jinqigufen.top

[S11] C：逐行读文件
来源：http://dvh.wangdashe.top

FILE *f = fopen("a.txt", "r");
来源：http://yyl.bjfxy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zbw.sweek.top

fclose(f);
来源：http://jup.daria6918.cn

[S12] C：写文件
来源：http://osl.sysykeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oio.nanxinkj.top

[S13] C：宏定义
来源：http://ejh.fzhhl.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://emk.daxiang520.top

[S14] C：枚举
来源：http://tbh.feifeiyinyue.top

enum Color { RED, GREEN, BLUE };
来源：http://qqu.chenjidiqi.icu

[S15] C：类型转换
来源：http://mdr.tian-w.cn

(double) a / b
来源：http://swz.cqqwz.cn

[S16] C：位操作置位
来源：http://gpp.shanyushiyangkeji.top

x |= (1 << 3);
来源：http://kpa.zdbjq.cn

[S17] C：安全拼接字符串
来源：http://euh.52xcode.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://prr.hywenlv.cn

[S18] C：命令行参数
来源：http://vkd.yongpay.top

int main(int argc, char **argv)
来源：http://yqy.svipenyu.cn

[S19] C：快速排序
来源：http://nfh.tianlin.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://csx.gaohongyu789.top

[S20] C：二分查找
来源：http://upl.hnqzz.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://czd.jyoumei.cn

[S21] C：字符类别判断
来源：http://itk.nanxinkj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zbf.smart0.xyz

[S22] C：字符串转数字
来源：http://iye.fehbvm.com

atoi("42");  strtod("3.14", NULL);
来源：http://zzt.fktsv.cn

[S23] C：随机数
来源：http://zgl.nanxinkj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rle.jianghu66.top

[S24] C：获取本地时间
来源：http://lrj.cashguo.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://puj.yongpay.top

[S25] C：内存拷贝
来源：http://ubz.svipenyu.cn

memcpy(dst, src, n);
来源：http://yvs.zdbjq.cn

[S26] C：内存清零
来源：http://avy.yangfankeji.com

memset(a, 0, sizeof a);
来源：http://fkp.ehwqpu.com

[S27] C：定义常量
来源：http://arz.xinyue.icu

const double PI = 3.14159;
来源：http://nbk.fzhhl.top

[S28] C：静态变量
来源：http://vwc.andypj.xyz

static int counter = 0;
来源：http://hyf.nanxinkj.top

[S29] C：变参函数
来源：http://fra.sufxvd.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dhz.daria6918.cn

[S30] C：头文件保护
来源：http://nrz.bjfxy.top

#ifndef X_H
来源：http://eur.jinyuanbaomall.cn

#define X_H
来源：http://rfk.fzhhl.top

#endif
来源：http://ydw.zhaomingkeji.xyz

[S31] C++：Hello World
来源：http://fqm.havefunace.top

#include <iostream>
来源：http://jie.zdqjudy.top

int main() { std::cout << "Hello\n"; }
来源：http://jtz.epnwcf.com

[S32] C++：字符串
来源：http://gxc.shanyushiyangkeji.top

std::string s = "hi";  s += "!";
来源：http://bxa.zhixingplan.top

[S33] C++：vector 增删
来源：http://tnq.jqgufenzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://evv.vqdsnc.cn

[S34] C++：遍历 vector
来源：http://zcv.hcnkem.com

for (auto &x : v) { std::cout << x; }
来源：http://hhi.wangdashe.top

[S35] C++：map
来源：http://fyp.dianchejie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://emo.gogol.net.cn

[S36] C++：unordered_map
来源：http://bhm.yfazqb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zrt.svipenyu.cn

[S37] C++：set
来源：http://qpr.cqqwz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kon.yfazqb.com

[S38] C++：排序
来源：http://fqk.jinqigufen.top

std::sort(v.begin(), v.end());
来源：http://gqz.hongshengwenyu.top

[S39] C++：自定义比较器排序
来源：http://nht.fengsongda.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://njo.zhixingplan.top

[S40] C++：查找元素
来源：http://cpm.cdnleiting.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lyf.cashguo.top

[S41] C++：类与构造函数
来源：http://oea.fktsv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://euv.jqgfzy.top

[S42] C++：继承与虚函数
来源：http://jhh.smart0.xyz

class B : public Base { public: void f() override {} };
来源：http://xkf.ydzc1.top

[S43] C++：智能指针
来源：http://jmt.uphjek.com

auto p = std::make_unique<int>(5);
来源：http://ubl.316326.xyz

[S44] C++：引用传参
来源：http://ihl.ydjk.org.cn

void inc(int &x) { ++x; }
来源：http://xas.yj202588.top

[S45] C++：lambda
来源：http://heh.dashuyun.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vps.shzxlz.cn

[S46] C++：函数模板
来源：http://cqg.chenlongwang.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vgp.hcnkem.com

[S47] C++：结构化绑定遍历
来源：http://voc.nwbrower.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pgb.hfpthk.cn

[S48] C++：逐行读文件
来源：http://dck.jiagoushi.top

std::ifstream in("a.txt");  std::string line;
来源：http://noe.hysaishi.cn

while (std::getline(in, line)) { }
来源：http://lqk.tianlin.xyz

[S49] C++：写文件
来源：http://oib.yvedp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ljd.ctjpmb.com

[S50] C++：格式化数字
来源：http://yyr.kuanghao11.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rtf.fehbvm.com

[S51] C++：显式类型转换
来源：http://hwo.yvedp.cn

static_cast<double>(a) / b
来源：http://net.mhx1999.top

[S52] C++：const 与 noexcept
来源：http://gvz.yongpay.top

int size() const noexcept { return n_; }
来源：http://wpx.xuetiantiany.cn

[S53] C++：移动语义
来源：http://pjl.zhengqikj.top

std::vector<int> w = std::move(v);
来源：http://xav.hnqzz.top

[S54] C++：异常处理
来源：http://fim.zycfv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fgq.jqgfzy.top

[S55] C++：结构化绑定
来源：http://mbi.yj20258.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vwq.xuetiantiany.cn

[S56] C++：optional
来源：http://dsp.gzhubu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xua.aizwys.cn

[S57] C++：编译期常量
来源：http://hui.bjfxy.top

constexpr int N = 10;
来源：http://eot.shuidangran.top

[S58] C++：命名空间
来源：http://fab.snrcjt.cn

namespace ns { int f() { return 1; } }
来源：http://cjw.daxiang520.top

[S59] C++：静态断言
来源：http://ujk.sjlbkw.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xza.0kj1m.cn

[S60] C++：遍历并删除元素
来源：http://bgr.nanxuanxn.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mci.snrcjt.cn

================================================================================
来源：http://vfo.sjlbkw.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://njz.sufxvd.cn

================================================================================
来源：http://bba.nanxuanxn.top

[T01] Kotlin：Hello World
来源：http://gpy.shangyingyoupin.top

println("Hello")
来源：http://dtk.jinghuilouyu.cn

[T02] Kotlin：变量
来源：http://qqu.cashguo.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uqu.hywenlv.cn

[T03] Kotlin：字符串模板
来源：http://myq.zhongyouzk.top

"值: $b"
来源：http://mku.jinqigfzy.top

[T04] Kotlin：空安全
来源：http://wim.birdmap.top

val n: String? = null;  n?.length
来源：http://epv.smart0.xyz


<!-- 参考信息 -->