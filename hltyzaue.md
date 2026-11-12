代发 wailian999

esac
来源：http://xzb.yvedp.cn

[R12] for 遍历文件
来源：http://eug.dianchejie.cn

for f in *.txt; do echo "$f"; done
来源：http://mwx.hywenlv.cn

[R13] for 计数循环
来源：http://tyf.ppjwa.cn

for i in {1..10}; do echo "$i"; done
来源：http://bjn.xuanzx.com

[R14] C 风格 for
来源：http://gyx.ivvv.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mdu.wangdashe.top

[R15] while 逐行读文件
来源：http://rts.nwbrower.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zce.daria6918.cn

[R16] until 等待条件
来源：http://fca.xuetiantiany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dmw.dashuyun.cn

[R17] 数组定义与取值
来源：http://xxf.shangyingyoupin.top

arr=(a b c); echo "${arr[0]}"
来源：http://hbj.gotoacloud.top

[R18] 遍历数组
来源：http://pet.ppjwa.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yuv.gaohongyu789.top

[R19] 数组长度
来源：http://lei.yuxming.cn

echo "${#arr[@]}"
来源：http://wwo.yuxming.cn

[R20] 关联数组（字典）
来源：http://jbo.pengpengdd.cyou

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dvx.chenlongwang.top

[R21] 字符串长度
来源：http://qlw.sxryk.cn

echo "${#s}"
来源：http://ofn.meibo888.top

[R22] 截取子串
来源：http://xxg.haohaochexian.top

echo "${s:0:5}"
来源：http://wre.chenjidiqi.icu

[R23] 字符串替换
来源：http://uan.quarkkingdee.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yhs.mhx1999.top

[R24] 大小写转换
来源：http://pst.ybcxt.top

echo "${s^^}"; echo "${s,,}"
来源：http://rco.yangfankeji.com

[R25] 去后缀 / 去前缀
来源：http://imq.52xcode.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gux.jiagoushi.top

[R26] 命令替换
来源：http://eks.smart0.xyz

now=$(date +%F); echo "$now"
来源：http://wgx.ydjk.org.cn

[R27] 算术展开
来源：http://xad.hnxiangtu.top

echo $((1 + 2 * 3))
来源：http://myi.hfpthk.cn

[R28] 浮点运算
来源：http://mky.wangdashe.top

echo "scale=2; 10/3" | bc
来源：http://vgd.chenzaomai.com

[R29] 定义函数
来源：http://ltw.cucudq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jej.jinghuilouyu.cn

[R30] 函数返回状态码
来源：http://kfm.snrcjt.cn

f() { return 0; }; f || echo "失败了"
来源：http://zgs.xylfe.cn

[R31] 局部变量
来源：http://ctw.iojbl.cn

f() { local x=1; echo "$x"; }
来源：http://kpi.svipenyu.cn

[R32] 参数个数校验
来源：http://azw.cucudq.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kpu.yueranfly.top

[R33] 捕获错误并提示行号
来源：http://yfd.52xcode.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uxu.chenjidiqi.icu

[R34] 退出时清理
来源：http://bfv.hongshengwenyu.top

trap 'rm -f "$tmp"' EXIT
来源：http://fls.daxiang520.top

[R35] 后台执行并等待
来源：http://xah.nanxuanxn.top

sleep 5 & pid=$!; wait "$pid"
来源：http://svh.nanxinkj.top

[R36] 并发执行多个任务
来源：http://oru.snrcjt.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nle.cheryme.top

[R37] 把输出赋给变量
来源：http://uaf.zdbjq.cn

files=$(ls -1)
来源：http://skj.fktsv.cn

[R38] 管道串联
来源：http://lou.wangdashe.top

cat a.txt | grep -i error | wc -l
来源：http://eca.zhijiandao.cn

[R39] 重定向标准输出与错误
来源：http://rjr.zhengqikj.top

cmd > out.log 2>&1
来源：http://akx.pycfn.com

[R40] 追加写日志
来源：http://gch.cheryme.top

echo "log" >> out.log
来源：http://idc.bjfxy.top

[R41] 丢弃输出
来源：http://poy.chenlongwang.top

cmd >/dev/null 2>&1
来源：http://ezd.bjfxy.top

[R42] 输入重定向
来源：http://irx.chenjidiqi.icu

wc -l < a.txt
来源：http://sao.xingfuxueyuan.xyz

[R43] 按名字查找文件
来源：http://smj.ivvv.top

find . -name "*.log" -type f
来源：http://dvd.cdnleiting.top

[R44] 按修改时间查找
来源：http://kpc.jinghuilouyu.cn

find . -mtime -7 -type f
来源：http://vpg.guowangkeji.top

[R45] 批量删除
来源：http://dgx.jqgufenzy.top

find . -name "*.tmp" -delete
来源：http://xec.nanxuanxn.top

[R46] 递归替换文件内容
来源：http://pix.ywan-chungtsiang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://avf.yonumen.top

[R47] sed 单行替换
来源：http://orx.jiagoushi.top

sed -i 's/foo/bar/g' a.txt
来源：http://dgf.fanxiaobao.xyz

[R48] awk 取指定列
来源：http://ehd.shuidangran.top

awk '{print $1, $3}' a.txt
来源：http://pbp.cqqwz.cn

[R49] awk 带条件
来源：http://dwr.yuxming.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pfm.bbcook.cn

[R50] awk 求和
来源：http://ipz.jianghu66.top

awk '{s += $2} END {print s}' a.txt
来源：http://whg.316326.xyz

[R51] 排序去重取前几
来源：http://vwl.epnwcf.com

sort a.txt | uniq -c | sort -rn | head
来源：http://ery.epnwcf.com

[R52] 统计行数
来源：http://bwl.dashuyun.cn

wc -l a.txt
来源：http://bja.hfpthk.cn

[R53] 查看文件头与实时尾
来源：http://xvl.guannengcc.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rgq.yfazqb.com

[R54] 比较两个文件
来源：http://jjr.hnqzz.top

diff a.txt b.txt
来源：http://cpv.meibo888.top

[R55] 压缩与解压
来源：http://tcq.nanxinkj.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://epj.fehbvm.com

[R56] 远程拷贝
来源：http://cqo.bbcook.cn

scp file user@host:/path/
来源：http://yrb.ehwqpu.com

[R57] 远程执行命令
来源：http://oon.birdmap.top

ssh user@host 'uptime'
来源：http://gge.guowangkeji.top

[R58] 下载文件
来源：http://fuv.aizwys.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://txk.jlsjyb.cn

[R59] 发 POST JSON
来源：http://neh.zdqjudy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hyq.uphjek.com

[R60] 只看 HTTP 状态码
来源：http://btw.hnxiangtu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uqv.guowangkeji.top

[R61] 磁盘占用
来源：http://vlf.tianlin.xyz

df -h;  du -sh *
来源：http://yil.svipenyu.cn

[R62] 找最占空间的文件
来源：http://trh.jiagoushi.top

du -ah . | sort -rh | head -10
来源：http://qab.yj20258.top

[R63] 内存与进程
来源：http://whd.hysaishi.cn

free -h;  ps aux | grep nginx
来源：http://anz.jinqigufen.top

[R64] 结束进程
来源：http://htj.andypj.xyz

kill -9 $(pgrep -f app.py)
来源：http://lae.nanxuanxn.top

[R65] 查看端口占用
来源：http://kbf.zycfv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eol.zhiwuduotai.top

[R66] 定时任务
来源：http://xsr.yvedp.cn

crontab -e;  crontab -l
来源：http://cko.52xcode.cn

[R67] 生成随机十六进制串
来源：http://wyt.jyoumei.cn

openssl rand -hex 16
来源：http://iql.fehbvm.com

[R68] 计算文件校验值
来源：http://wgx.zhongyouzk.top

sha256sum a.txt;  md5sum a.txt
来源：http://sxp.ppjwa.cn

[R69] 生成随机密码
来源：http://mqv.andypj.xyz

head -c 16 /dev/urandom | base64
来源：http://ekf.guowangkeji.top

[R70] 时间戳与互转
来源：http://tzr.yonumen.top

date +%s;  date -d @1700000000
来源：http://hmd.yonumen.top

[R71] 日期格式化
来源：http://pyg.hywenlv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://agi.ppjwa.cn

[R72] 等待端口就绪
来源：http://gmx.zhiwuduotai.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wgs.ywan-chungtsiang.top

[R73] 分割大日志
来源：http://ktd.sjlbkw.cn

split -l 1000 big.log part_
来源：http://gdz.xingfuxueyuan.xyz

[R74] 批量重命名
来源：http://cdp.chenlongwang.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://otv.redwolf501.top

[R75] 导出环境变量
来源：http://xgt.fktsv.cn

export PATH="$HOME/bin:$PATH"
来源：http://iqe.ydjk.org.cn

[R76] 使用临时文件
来源：http://zvy.zhongyouzk.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nod.xuanzx.com

[R77] 读取用户输入
来源：http://xmj.yuxming.cn

read -rp "请输入: " ans
来源：http://jlg.c1oappe.top

[R78] 交互式菜单
来源：http://uao.gaohongyu789.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wji.ydjk.org.cn

[R79] 解析命令行选项
来源：http://ria.haohaochexian.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hfw.nwbrower.top

[R80] 查看脚本执行耗时
来源：http://vlj.zhixingplan.top

time ./run.sh
来源：http://gzf.yvedp.cn

================================================================================
来源：http://fzz.cdnleiting.top

S. C / C++ 专题
来源：http://jyu.ppjwa.cn

================================================================================
来源：http://ldb.xylfe.cn

[S01] C：Hello World
来源：http://lue.wangshuangyany.cn

#include <stdio.h>
来源：http://byt.zhongyouzk.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://pgz.yfazqb.com

[S02] C：变量与格式化输出
来源：http://syn.shzxlz.cn

int a = 10; printf("%d\n", a);
来源：http://ggb.jyoumei.cn

[S03] C：读入整数
来源：http://tvg.jinqigfzy.top

int x; scanf("%d", &x);
来源：http://eei.yonumen.top

[S04] C：字符串复制
来源：http://jud.nwbrower.top

char dst[32]; strcpy(dst, "hi");
来源：http://zyy.tanke756.top

[S05] C：字符串长度
来源：http://yjn.sxryk.cn

strlen(s)
来源：http://zpe.zhoulong.xyz

[S06] C：字符串比较
来源：http://djs.guowangkeji.top

strcmp(a, b) == 0
来源：http://jef.jianghu66.top

[S07] C：数组遍历求和
来源：http://crp.jlsjyb.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vlb.uphjek.com

[S08] C：动态内存分配与释放
来源：http://edn.tanke756.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fky.yueranfly.top

[S09] C：结构体定义与初始化
来源：http://wsh.shangyingyoupin.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pbr.ctjpmb.com

[S10] C：指针与解引用
来源：http://rpa.vehdjk.com

int *p = &a;  *p = 5;
来源：http://xpj.ydjk.org.cn

[S11] C：逐行读文件
来源：http://ldy.smart0.xyz

FILE *f = fopen("a.txt", "r");
来源：http://rxr.ywan-chungtsiang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zlk.feifeiyinyue.top

fclose(f);
来源：http://fzi.zhiwuduotai.top

[S12] C：写文件
来源：http://nhm.hywenlv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ghl.xylfe.cn

[S13] C：宏定义
来源：http://prz.tarul.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cbp.zhengqikj.top

[S14] C：枚举
来源：http://hss.svipenyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://duv.xylfe.cn

[S15] C：类型转换
来源：http://now.daria6918.cn

(double) a / b
来源：http://pan.ydjk.org.cn

[S16] C：位操作置位
来源：http://glr.yueranfly.top

x |= (1 << 3);
来源：http://osz.yanxiufei.cn

[S17] C：安全拼接字符串
来源：http://uki.fehbvm.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gcs.jinghuilouyu.cn

[S18] C：命令行参数
来源：http://dim.wangdashe.top

int main(int argc, char **argv)
来源：http://gay.guannengcc.top

[S19] C：快速排序
来源：http://fws.jinqigufen.top

qsort(a, n, sizeof(int), cmp);
来源：http://lnl.vehdjk.com

[S20] C：二分查找
来源：http://ack.bjfxy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://enf.zdbjq.cn

[S21] C：字符类别判断
来源：http://rpd.pycfn.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xvz.cqqwz.cn

[S22] C：字符串转数字
来源：http://kqc.hammf.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dts.guannengcc.top

[S23] C：随机数
来源：http://kvo.hfpthk.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hlm.uphjek.com

[S24] C：获取本地时间
来源：http://vhj.tanke756.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lcn.vehdjk.com

[S25] C：内存拷贝
来源：http://azc.sufxvd.cn

memcpy(dst, src, n);
来源：http://upw.vqdsnc.cn

[S26] C：内存清零
来源：http://nwg.hesvh.cn

memset(a, 0, sizeof a);
来源：http://faf.aibaodan.cn

[S27] C：定义常量
来源：http://mam.bbcook.cn

const double PI = 3.14159;
来源：http://hjj.c1oappe.top

[S28] C：静态变量
来源：http://spx.hysaishi.cn

static int counter = 0;
来源：http://bvt.quarkkingdee.top

[S29] C：变参函数
来源：http://fkx.havefunace.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wsv.yj202588.top

[S30] C：头文件保护
来源：http://epq.tianlin.xyz

#ifndef X_H
来源：http://vyc.tian-w.cn

#define X_H
来源：http://tia.fengsongda.top

#endif
来源：http://ahl.snrcjt.cn

[S31] C++：Hello World
来源：http://oab.ppjwa.cn

#include <iostream>
来源：http://wvz.chenlongwang.top

int main() { std::cout << "Hello\n"; }
来源：http://xsh.gogol.net.cn

[S32] C++：字符串
来源：http://pnv.nanxinkj.top

std::string s = "hi";  s += "!";
来源：http://bdt.zhongyouzk.top

[S33] C++：vector 增删
来源：http://nzt.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eia.snrcjt.cn

[S34] C++：遍历 vector
来源：http://vxv.epnwcf.com

for (auto &x : v) { std::cout << x; }
来源：http://qqn.uphjek.com

[S35] C++：map
来源：http://yjm.xingfuxueyuan.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tdn.ppjwa.cn

[S36] C++：unordered_map
来源：http://ysx.hnxiangtu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jdn.wangdashe.top

[S37] C++：set
来源：http://dqo.uphjek.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vgc.yongpay.top

[S38] C++：排序
来源：http://ekz.pengpengdd.cyou

std::sort(v.begin(), v.end());
来源：http://thx.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://hac.yangfankeji.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iai.ydjk.org.cn

[S40] C++：查找元素
来源：http://luz.bbcook.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xrs.cheryme.top

[S41] C++：类与构造函数
来源：http://urq.xinyue.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jad.ivvv.top

[S42] C++：继承与虚函数
来源：http://mdu.aibaodan.cn

class B : public Base { public: void f() override {} };
来源：http://ovm.zhaomingkeji.xyz

[S43] C++：智能指针
来源：http://qen.yj202588.top

auto p = std::make_unique<int>(5);
来源：http://bkj.chenjidiqi.icu

[S44] C++：引用传参
来源：http://nzd.c1oappe.top

void inc(int &x) { ++x; }
来源：http://vev.jinyuanbaomall.cn

[S45] C++：lambda
来源：http://xil.xylfe.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bof.hongshengwenyu.top

[S46] C++：函数模板
来源：http://pvn.smart0.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bqb.fehbvm.com

[S47] C++：结构化绑定遍历
来源：http://nlm.yj20258888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ukg.hammf.cn

[S48] C++：逐行读文件
来源：http://doy.zdbjq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zmb.jinqigfzy.top

while (std::getline(in, line)) { }
来源：http://ymy.xziqi.cn

[S49] C++：写文件
来源：http://ewu.hfpthk.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gfw.jinyuanbaomall.cn

[S50] C++：格式化数字
来源：http://wrk.yonumen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mwu.hnxiangtu.top

[S51] C++：显式类型转换
来源：http://jci.shangyingyoupin.top

static_cast<double>(a) / b
来源：http://inc.sweek.top

[S52] C++：const 与 noexcept
来源：http://ijt.zhiwuduotai.top

int size() const noexcept { return n_; }
来源：http://kxe.hnxiangtu.top

[S53] C++：移动语义
来源：http://ssk.nwbrower.top

std::vector<int> w = std::move(v);
来源：http://cbe.yongpay.top

[S54] C++：异常处理
来源：http://tgz.pycfn.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fiq.jinyuanbaomall.cn

[S55] C++：结构化绑定
来源：http://lwh.redwolf501.top

auto [a, b] = std::make_pair(1, 2);
来源：http://udq.tanke756.top

[S56] C++：optional
来源：http://rgd.daria6918.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jcd.yuanzhike.top

[S57] C++：编译期常量
来源：http://qtv.jinqigufen.top

constexpr int N = 10;
来源：http://uuq.xuetiantiany.cn

[S58] C++：命名空间
来源：http://ldh.316326.xyz

namespace ns { int f() { return 1; } }
来源：http://ngc.xingfuxueyuan.xyz

[S59] C++：静态断言
来源：http://epe.yonumen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gza.chenjidiqi.icu

[S60] C++：遍历并删除元素
来源：http://ipu.shzxlz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hlo.shangyingyoupin.top

================================================================================
来源：http://age.jlsjyb.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qli.zhiwuduotai.top

================================================================================
来源：http://hev.jinghuilouyu.cn

[T01] Kotlin：Hello World
来源：http://sch.yvedp.cn

println("Hello")
来源：http://uod.chenjidiqi.icu

[T02] Kotlin：变量
来源：http://vif.yj20258.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kvl.svipenyu.cn

[T03] Kotlin：字符串模板
来源：http://tqc.cheryme.top

"值: $b"
来源：http://rrd.xuetiantiany.cn

[T04] Kotlin：空安全
来源：http://vhe.sweek.top

val n: String? = null;  n?.length
来源：http://jwi.bjfxy.top

[T05] Kotlin：when 表达式
来源：http://pyw.xuetiantiany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ics.316326.xyz

[T06] Kotlin：集合映射
来源：http://nzr.ydzc1.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vkx.hcnkem.com

[T07] Kotlin：集合过滤
来源：http://sad.svipenyu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gmw.yfazqb.com

[T08] Kotlin：数据类
来源：http://hiy.zhiwuduotai.top

data class User(val name: String, val age: Int)
来源：http://bsl.sweek.top

[T09] Kotlin：扩展函数
来源：http://vyj.zhixingplan.top

fun String.exclaim() = this + "!"
来源：http://ong.chenzaomai.com

[T10] Kotlin：默认参数
来源：http://szl.zhengqikj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://fbg.iojbl.cn

[T11] Kotlin：协程
来源：http://igv.fengsongda.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gti.bbcook.cn

[T12] Kotlin：解构声明
来源：http://dds.zhengqikj.top

val (a, b) = Pair(1, 2)
来源：http://eby.sjlbkw.cn

[T13] Kotlin：只读 Map
来源：http://poe.hfpthk.cn

val m = mapOf("a" to 1)
来源：http://dtg.guannengcc.top

[T14] Kotlin：循环
来源：http://ubo.xuetiantiany.cn

for (i in 1..10) println(i)
来源：http://psm.hnqzz.top


<!-- 参考信息 -->