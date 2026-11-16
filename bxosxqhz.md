代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lvy.zhoulong.xyz

[R08] 数值比较
来源：http://obs.yonumen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rqb.jlsjyb.cn

[R09] 字符串比较
来源：http://nsq.hnqzz.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vwe.yanxiufei.cn

[R10] 正则匹配
来源：http://ahn.shuidangran.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pig.bbcook.cn

[R11] case 多分支
来源：http://htr.nanxinkj.top

case "$1" in
来源：http://vzq.ppjwa.cn

start) echo "启动" ;;
来源：http://rfa.mhx1999.top

stop)  echo "停止" ;;
来源：http://mep.daria6918.cn

*)     echo "未知命令" ;;
来源：http://cca.yvedp.cn

esac
来源：http://mdi.dashuyun.cn

[R12] for 遍历文件
来源：http://hji.jiagoushi.top

for f in *.txt; do echo "$f"; done
来源：http://pxl.yonumen.top

[R13] for 计数循环
来源：http://cdk.zhongyouzk.top

for i in {1..10}; do echo "$i"; done
来源：http://foj.ppjwa.cn

[R14] C 风格 for
来源：http://ake.zdqjudy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gct.xuetiantiany.cn

[R15] while 逐行读文件
来源：http://djc.vqdsnc.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pbl.c1oappe.top

[R16] until 等待条件
来源：http://zdb.nanxinkj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iwa.daxiang520.top

[R17] 数组定义与取值
来源：http://gth.snrcjt.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wry.sxryk.cn

[R18] 遍历数组
来源：http://nua.tanke756.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zxz.quarkkingdee.top

[R19] 数组长度
来源：http://pkx.nanxinkj.top

echo "${#arr[@]}"
来源：http://hwm.xylfe.cn

[R20] 关联数组（字典）
来源：http://lnu.tarul.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gnu.jqgfzy.top

[R21] 字符串长度
来源：http://dqx.gotoacloud.top

echo "${#s}"
来源：http://bpu.snrcjt.cn

[R22] 截取子串
来源：http://uza.smart0.xyz

echo "${s:0:5}"
来源：http://skm.aibaodan.cn

[R23] 字符串替换
来源：http://qmg.yuanzhike.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://trm.fzhhl.top

[R24] 大小写转换
来源：http://xqr.zhiwuduotai.top

echo "${s^^}"; echo "${s,,}"
来源：http://hrg.fanxiaobao.xyz

[R25] 去后缀 / 去前缀
来源：http://ukv.zhongyouzk.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fdo.fengsongda.top

[R26] 命令替换
来源：http://urw.9152youxi.cn

now=$(date +%F); echo "$now"
来源：http://pug.hammf.cn

[R27] 算术展开
来源：http://rxi.jqgufenzy.top

echo $((1 + 2 * 3))
来源：http://jee.yj202588.top

[R28] 浮点运算
来源：http://vdg.yj202588.top

echo "scale=2; 10/3" | bc
来源：http://qdz.cashguo.top

[R29] 定义函数
来源：http://wye.chenlongwang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lxs.vehdjk.com

[R30] 函数返回状态码
来源：http://sxn.pycfn.com

f() { return 0; }; f || echo "失败了"
来源：http://idg.cdnleiting.top

[R31] 局部变量
来源：http://kru.xziqi.cn

f() { local x=1; echo "$x"; }
来源：http://tdu.zhixingplan.top

[R32] 参数个数校验
来源：http://gna.yj202588.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://olr.xinyue.icu

[R33] 捕获错误并提示行号
来源：http://kxg.yuanzhike.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hsv.0kj1m.cn

[R34] 退出时清理
来源：http://khu.ppjwa.cn

trap 'rm -f "$tmp"' EXIT
来源：http://phg.yj20258.top

[R35] 后台执行并等待
来源：http://pco.meibo888.top

sleep 5 & pid=$!; wait "$pid"
来源：http://lux.wangdashe.top

[R36] 并发执行多个任务
来源：http://alo.c1oappe.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yzd.yj202588.top

[R37] 把输出赋给变量
来源：http://fzy.ywan-chungtsiang.top

files=$(ls -1)
来源：http://zrh.fehbvm.com

[R38] 管道串联
来源：http://uye.ybcxt.top

cat a.txt | grep -i error | wc -l
来源：http://tfb.wangdashe.top

[R39] 重定向标准输出与错误
来源：http://uhz.ehwqpu.com

cmd > out.log 2>&1
来源：http://aik.fehbvm.com

[R40] 追加写日志
来源：http://qys.chenjidiqi.icu

echo "log" >> out.log
来源：http://cku.yj202588.top

[R41] 丢弃输出
来源：http://sry.fktsv.cn

cmd >/dev/null 2>&1
来源：http://gzh.cucudq.cn

[R42] 输入重定向
来源：http://obq.dianchejie.cn

wc -l < a.txt
来源：http://rvr.jinqigufen.top

[R43] 按名字查找文件
来源：http://qsf.tianlin.xyz

find . -name "*.log" -type f
来源：http://yfz.vehdjk.com

[R44] 按修改时间查找
来源：http://uhm.9152youxi.cn

find . -mtime -7 -type f
来源：http://paw.yfazqb.com

[R45] 批量删除
来源：http://qld.fengsongda.top

find . -name "*.tmp" -delete
来源：http://grr.ydjk.org.cn

[R46] 递归替换文件内容
来源：http://rdf.quarkkingdee.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kmm.shangyingyoupin.top

[R47] sed 单行替换
来源：http://rrg.ywan-chungtsiang.top

sed -i 's/foo/bar/g' a.txt
来源：http://liu.jianghu66.top

[R48] awk 取指定列
来源：http://vcy.dianchejie.cn

awk '{print $1, $3}' a.txt
来源：http://dcb.shangyingyoupin.top

[R49] awk 带条件
来源：http://pic.tarul.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ndj.xylfe.cn

[R50] awk 求和
来源：http://brq.gaohongyu789.top

awk '{s += $2} END {print s}' a.txt
来源：http://djh.cheryme.top

[R51] 排序去重取前几
来源：http://nvp.shangyingyoupin.top

sort a.txt | uniq -c | sort -rn | head
来源：http://xym.haohaochexian.top

[R52] 统计行数
来源：http://zng.bbcook.cn

wc -l a.txt
来源：http://tpy.jqgufenzy.top

[R53] 查看文件头与实时尾
来源：http://kpc.daxiang520.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gkp.ydzc1.top

[R54] 比较两个文件
来源：http://zbw.shuidangran.top

diff a.txt b.txt
来源：http://mpj.ydjk.org.cn

[R55] 压缩与解压
来源：http://tuu.yangfankeji.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kyq.jyoumei.cn

[R56] 远程拷贝
来源：http://ztz.andypj.xyz

scp file user@host:/path/
来源：http://gnz.ydzc1.top

[R57] 远程执行命令
来源：http://vcd.zdqjudy.top

ssh user@host 'uptime'
来源：http://ebz.wangdashe.top

[R58] 下载文件
来源：http://rac.nwbrower.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dja.hysaishi.cn

[R59] 发 POST JSON
来源：http://sbd.zhaomingkeji.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wvt.0kj1m.cn

[R60] 只看 HTTP 状态码
来源：http://gwj.cheryme.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zyy.ybcxt.top

[R61] 磁盘占用
来源：http://knh.zdqjudy.top

df -h;  du -sh *
来源：http://rgx.316326.xyz

[R62] 找最占空间的文件
来源：http://jkc.yj20258888.top

du -ah . | sort -rh | head -10
来源：http://evw.feifeiyinyue.top

[R63] 内存与进程
来源：http://ter.havefunace.top

free -h;  ps aux | grep nginx
来源：http://req.iojbl.cn

[R64] 结束进程
来源：http://ifh.fanxiaobao.xyz

kill -9 $(pgrep -f app.py)
来源：http://tdh.316326.xyz

[R65] 查看端口占用
来源：http://kep.chenjidiqi.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://evk.nanxuanxn.top

[R66] 定时任务
来源：http://hzk.hammf.cn

crontab -e;  crontab -l
来源：http://axv.cashguo.top

[R67] 生成随机十六进制串
来源：http://vep.nwbrower.top

openssl rand -hex 16
来源：http://cla.316326.xyz

[R68] 计算文件校验值
来源：http://dxm.sysykeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://ost.yanxiufei.cn

[R69] 生成随机密码
来源：http://psj.hammf.cn

head -c 16 /dev/urandom | base64
来源：http://oai.cashguo.top

[R70] 时间戳与互转
来源：http://iyn.yonumen.top

date +%s;  date -d @1700000000
来源：http://xnh.aizwys.cn

[R71] 日期格式化
来源：http://odi.zdbjq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rht.hfpthk.cn

[R72] 等待端口就绪
来源：http://nzr.svipenyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mtk.jinqigufen.top

[R73] 分割大日志
来源：http://pnj.svipenyu.cn

split -l 1000 big.log part_
来源：http://vtj.jqgfzy.top

[R74] 批量重命名
来源：http://vwp.daria6918.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://htk.yj202588.top

[R75] 导出环境变量
来源：http://yyf.fzhhl.top

export PATH="$HOME/bin:$PATH"
来源：http://ncn.tarul.cn

[R76] 使用临时文件
来源：http://tuc.nanxinkj.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kfe.jyoumei.cn

[R77] 读取用户输入
来源：http://fgv.zhixingplan.top

read -rp "请输入: " ans
来源：http://yct.hfpthk.cn

[R78] 交互式菜单
来源：http://uuy.fanxiaobao.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://wep.hnxiangtu.top

[R79] 解析命令行选项
来源：http://abe.fzhhl.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://css.kuanghao11.cn

[R80] 查看脚本执行耗时
来源：http://ojx.dashuyun.cn

time ./run.sh
来源：http://fuj.c1oappe.top

================================================================================
来源：http://rcf.zycfv.cn

S. C / C++ 专题
来源：http://lcz.tanke756.top

================================================================================
来源：http://tfj.zycfv.cn

[S01] C：Hello World
来源：http://hhk.tian-w.cn

#include <stdio.h>
来源：http://wgd.haohaochexian.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://prp.vehdjk.com

[S02] C：变量与格式化输出
来源：http://bbz.vehdjk.com

int a = 10; printf("%d\n", a);
来源：http://voo.yongpay.top

[S03] C：读入整数
来源：http://krm.yvedp.cn

int x; scanf("%d", &x);
来源：http://wnw.sjlbkw.cn

[S04] C：字符串复制
来源：http://wzb.sweek.top

char dst[32]; strcpy(dst, "hi");
来源：http://chs.bjfxy.top

[S05] C：字符串长度
来源：http://ejy.hysaishi.cn

strlen(s)
来源：http://oep.fanxiaobao.xyz

[S06] C：字符串比较
来源：http://oau.jiagoushi.top

strcmp(a, b) == 0
来源：http://qcn.birdmap.top

[S07] C：数组遍历求和
来源：http://wvw.316326.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://llr.sweek.top

[S08] C：动态内存分配与释放
来源：http://npc.ybcxt.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lja.hongshengwenyu.top

[S09] C：结构体定义与初始化
来源：http://bwh.guannengcc.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gkl.jqgufenzy.top

[S10] C：指针与解引用
来源：http://uwg.hfpthk.cn

int *p = &a;  *p = 5;
来源：http://cua.xuetiantiany.cn

[S11] C：逐行读文件
来源：http://bby.fehbvm.com

FILE *f = fopen("a.txt", "r");
来源：http://xrx.zhongyouzk.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xfo.ywan-chungtsiang.top

fclose(f);
来源：http://toe.jinqigufen.top

[S12] C：写文件
来源：http://ffx.hnxiangtu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://awq.zhengqikj.top

[S13] C：宏定义
来源：http://tau.tanke756.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ilz.yj202588.top

[S14] C：枚举
来源：http://ouc.zdbjq.cn

enum Color { RED, GREEN, BLUE };
来源：http://jyo.hammf.cn

[S15] C：类型转换
来源：http://gmj.ywan-chungtsiang.top

(double) a / b
来源：http://dgw.ybcxt.top

[S16] C：位操作置位
来源：http://boq.zhijiandao.cn

x |= (1 << 3);
来源：http://zoh.sweek.top

[S17] C：安全拼接字符串
来源：http://kaj.zhaomingkeji.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wsx.fktsv.cn

[S18] C：命令行参数
来源：http://kmu.pengpengdd.cyou

int main(int argc, char **argv)
来源：http://mtt.dashuyun.cn

[S19] C：快速排序
来源：http://wbi.guannengcc.top

qsort(a, n, sizeof(int), cmp);
来源：http://bnl.havefunace.top

[S20] C：二分查找
来源：http://sxw.wangdashe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wlk.ybcxt.top

[S21] C：字符类别判断
来源：http://ffh.tanke756.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://aos.shanyushiyangkeji.top

[S22] C：字符串转数字
来源：http://wtv.bbcook.cn

atoi("42");  strtod("3.14", NULL);
来源：http://grl.haohaochexian.top

[S23] C：随机数
来源：http://fys.jinyuanbaomall.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pvq.yuanzhike.top

[S24] C：获取本地时间
来源：http://sts.shzxlz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mld.yj20258888.top

[S25] C：内存拷贝
来源：http://jzz.gogol.net.cn

memcpy(dst, src, n);
来源：http://feg.sufxvd.cn

[S26] C：内存清零
来源：http://rij.ydjk.org.cn

memset(a, 0, sizeof a);
来源：http://txu.xuetiantiany.cn

[S27] C：定义常量
来源：http://yzt.jinqigufen.top

const double PI = 3.14159;
来源：http://txu.havefunace.top

[S28] C：静态变量
来源：http://pcy.yangfankeji.com

static int counter = 0;
来源：http://cuo.gogol.net.cn

[S29] C：变参函数
来源：http://nxd.sufxvd.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pih.ivvv.top

[S30] C：头文件保护
来源：http://pyw.yj20258888.top

#ifndef X_H
来源：http://nqv.ppjwa.cn

#define X_H
来源：http://skm.fzhhl.top

#endif
来源：http://gpx.jqgufenzy.top

[S31] C++：Hello World
来源：http://cmn.ivvv.top

#include <iostream>
来源：http://znb.chenzaomai.com

int main() { std::cout << "Hello\n"; }
来源：http://eqc.yonumen.top

[S32] C++：字符串
来源：http://xms.hcnkem.com

std::string s = "hi";  s += "!";
来源：http://vch.yj20258888.top

[S33] C++：vector 增删
来源：http://wmj.zdbjq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://brt.tianlin.xyz

[S34] C++：遍历 vector
来源：http://txu.sjlbkw.cn

for (auto &x : v) { std::cout << x; }
来源：http://uba.gaohongyu789.top

[S35] C++：map
来源：http://xfd.dianchejie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gun.hywenlv.cn

[S36] C++：unordered_map
来源：http://tam.sweek.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qnt.shanyushiyangtech.top

[S37] C++：set
来源：http://lij.yangfankeji.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mmu.svipenyu.cn

[S38] C++：排序
来源：http://kcv.wangdashe.top

std::sort(v.begin(), v.end());
来源：http://ouu.sjlbkw.cn

[S39] C++：自定义比较器排序
来源：http://gbl.xuetiantiany.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gab.shzxlz.cn

[S40] C++：查找元素
来源：http://jet.xuetiantiany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://srl.hcnkem.com

[S41] C++：类与构造函数
来源：http://hma.chenjidiqi.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hmd.shuidangran.top

[S42] C++：继承与虚函数
来源：http://zzh.gogol.net.cn

class B : public Base { public: void f() override {} };
来源：http://dbq.andypj.xyz

[S43] C++：智能指针
来源：http://hal.yj202588.top

auto p = std::make_unique<int>(5);
来源：http://fug.shanyushiyangtech.top

[S44] C++：引用传参
来源：http://cdf.fktsv.cn

void inc(int &x) { ++x; }
来源：http://hfr.yangfankeji.com

[S45] C++：lambda
来源：http://zvo.dianchejie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ayw.birdmap.top

[S46] C++：函数模板
来源：http://dsh.guowangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oww.zdbjq.cn

[S47] C++：结构化绑定遍历
来源：http://ydt.sysykeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qzh.shzxlz.cn

[S48] C++：逐行读文件
来源：http://lbp.chenjidiqi.icu

std::ifstream in("a.txt");  std::string line;
来源：http://mmb.aibaodan.cn

while (std::getline(in, line)) { }
来源：http://ouq.yueranfly.top

[S49] C++：写文件
来源：http://fzs.guannengcc.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tij.52xcode.cn

[S50] C++：格式化数字
来源：http://ynd.cheryme.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xlk.hnxiangtu.top

[S51] C++：显式类型转换
来源：http://cfa.quarkkingdee.top

static_cast<double>(a) / b
来源：http://pir.fktsv.cn

[S52] C++：const 与 noexcept
来源：http://bsb.cashguo.top

int size() const noexcept { return n_; }
来源：http://pfw.hnqzz.top

[S53] C++：移动语义
来源：http://vwe.yj20258888.top

std::vector<int> w = std::move(v);
来源：http://boh.jiagoushi.top

[S54] C++：异常处理
来源：http://syl.gogol.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nij.jinqigfzy.top

[S55] C++：结构化绑定
来源：http://xbs.xuanzx.com

auto [a, b] = std::make_pair(1, 2);
来源：http://rxq.ybcxt.top

[S56] C++：optional
来源：http://poz.uphjek.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://adq.pycfn.com

[S57] C++：编译期常量
来源：http://zms.zhiwuduotai.top

constexpr int N = 10;
来源：http://wvk.tian-w.cn

[S58] C++：命名空间
来源：http://hyz.vqdsnc.cn

namespace ns { int f() { return 1; } }
来源：http://der.meibo888.top

[S59] C++：静态断言
来源：http://idd.jlsjyb.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://siz.zhoulong.xyz

[S60] C++：遍历并删除元素
来源：http://pbc.9152youxi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oda.c1oappe.top

================================================================================
来源：http://wlt.jiagoushi.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ita.zdqjudy.top

================================================================================
来源：http://qxx.shzxlz.cn

[T01] Kotlin：Hello World
来源：http://rur.nwbrower.top

println("Hello")
来源：http://ggs.daria6918.cn

[T02] Kotlin：变量
来源：http://fvr.mhx1999.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jjz.gaohongyu789.top

[T03] Kotlin：字符串模板
来源：http://die.jinqigfzy.top

"值: $b"
来源：http://seu.jyoumei.cn

[T04] Kotlin：空安全
来源：http://noy.0kj1m.cn

val n: String? = null;  n?.length
来源：http://toc.yongpay.top

[T05] Kotlin：when 表达式
来源：http://wea.9152youxi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jjl.daria6918.cn

[T06] Kotlin：集合映射
来源：http://zan.nanxuanxn.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tqz.ydzc1.top

[T07] Kotlin：集合过滤
来源：http://hno.ppjwa.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vpj.chenlongwang.top

[T08] Kotlin：数据类
来源：http://rah.ywan-chungtsiang.top

data class User(val name: String, val age: Int)
来源：http://lrx.shanyushiyangkeji.top


<!-- 参考信息 -->