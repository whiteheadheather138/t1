代发 wailian999

set -euo pipefail
来源：http://chz.jinghuilouyu.cn

[R02] 变量赋值与使用
来源：http://vjs.pengpengdd.cyou

name="Tom"; echo "$name"
来源：http://eyn.cqqwz.cn

[R03] 只读变量
来源：http://sql.mhx1999.top

readonly PI=3.14
来源：http://idd.wangshuangyany.cn

[R04] 位置参数
来源：http://kfy.daria6918.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://usn.daxiang520.top

[R05] 参数默认值
来源：http://foh.hnxiangtu.top

name="${1:-default}"
来源：http://hvk.yangfankeji.com

[R06] 判断命令是否存在
来源：http://cxe.zdqjudy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fjt.wangshuangyany.cn

[R07] if 判断文件
来源：http://hcj.hysaishi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://knz.hfpthk.cn

[R08] 数值比较
来源：http://wga.wangshuangyany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nzb.cucudq.cn

[R09] 字符串比较
来源：http://qpp.dashuyun.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yqx.gogol.net.cn

[R10] 正则匹配
来源：http://uwq.fanxiaobao.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pnd.xuanzx.com

[R11] case 多分支
来源：http://pgk.daria6918.cn

case "$1" in
来源：http://hgb.ydzc1.top

start) echo "启动" ;;
来源：http://vtc.sweek.top

stop)  echo "停止" ;;
来源：http://hwy.0kj1m.cn

*)     echo "未知命令" ;;
来源：http://eez.ydjk.org.cn

esac
来源：http://bkr.jqgufenzy.top

[R12] for 遍历文件
来源：http://olh.feifeiyinyue.top

for f in *.txt; do echo "$f"; done
来源：http://vjd.shangyingyoupin.top

[R13] for 计数循环
来源：http://shr.zhongyouzk.top

for i in {1..10}; do echo "$i"; done
来源：http://osd.jyoumei.cn

[R14] C 风格 for
来源：http://vsy.yueranfly.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sue.zhaomingkeji.xyz

[R15] while 逐行读文件
来源：http://pxk.svipenyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tqt.feifeiyinyue.top

[R16] until 等待条件
来源：http://ryo.chenlongwang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hsl.hcnkem.com

[R17] 数组定义与取值
来源：http://feb.c1oappe.top

arr=(a b c); echo "${arr[0]}"
来源：http://rxe.316326.xyz

[R18] 遍历数组
来源：http://eum.cdnleiting.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zib.fanxiaobao.xyz

[R19] 数组长度
来源：http://mfq.daria6918.cn

echo "${#arr[@]}"
来源：http://mxf.ivvv.top

[R20] 关联数组（字典）
来源：http://tcm.cdnleiting.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ndl.xuanzx.com

[R21] 字符串长度
来源：http://odm.xziqi.cn

echo "${#s}"
来源：http://sny.pengpengdd.cyou

[R22] 截取子串
来源：http://iak.sjlbkw.cn

echo "${s:0:5}"
来源：http://nbv.daxiang520.top

[R23] 字符串替换
来源：http://avj.hcnkem.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uzp.yj202588.top

[R24] 大小写转换
来源：http://qbc.bbcook.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uzx.316326.xyz

[R25] 去后缀 / 去前缀
来源：http://tav.jinghuilouyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hoa.hywenlv.cn

[R26] 命令替换
来源：http://hgp.ivvv.top

now=$(date +%F); echo "$now"
来源：http://sfl.feifeiyinyue.top

[R27] 算术展开
来源：http://fpp.shuidangran.top

echo $((1 + 2 * 3))
来源：http://ixa.jqgfzy.top

[R28] 浮点运算
来源：http://buu.gaohongyu789.top

echo "scale=2; 10/3" | bc
来源：http://aei.tianlin.xyz

[R29] 定义函数
来源：http://htg.epnwcf.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tiu.fanxiaobao.xyz

[R30] 函数返回状态码
来源：http://wnt.mhx1999.top

f() { return 0; }; f || echo "失败了"
来源：http://nbc.yonumen.top

[R31] 局部变量
来源：http://wjl.xinyue.icu

f() { local x=1; echo "$x"; }
来源：http://rlo.hnqzz.top

[R32] 参数个数校验
来源：http://xeg.ybcxt.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zdl.quarkkingdee.top

[R33] 捕获错误并提示行号
来源：http://vgd.fzhhl.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tyk.ivvv.top

[R34] 退出时清理
来源：http://obb.tian-w.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ojw.meibo888.top

[R35] 后台执行并等待
来源：http://mzh.hywenlv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pya.jlsjyb.cn

[R36] 并发执行多个任务
来源：http://kyx.guowangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eff.zhoulong.xyz

[R37] 把输出赋给变量
来源：http://asw.zhoulong.xyz

files=$(ls -1)
来源：http://cwf.quarkkingdee.top

[R38] 管道串联
来源：http://ugx.smart0.xyz

cat a.txt | grep -i error | wc -l
来源：http://enr.zhoulong.xyz

[R39] 重定向标准输出与错误
来源：http://mdt.cdnleiting.top

cmd > out.log 2>&1
来源：http://odd.jlsjyb.cn

[R40] 追加写日志
来源：http://jiv.jqgfzy.top

echo "log" >> out.log
来源：http://bkz.havefunace.top

[R41] 丢弃输出
来源：http://mps.pycfn.com

cmd >/dev/null 2>&1
来源：http://abn.jinqigufen.top

[R42] 输入重定向
来源：http://wdi.hesvh.cn

wc -l < a.txt
来源：http://bas.sufxvd.cn

[R43] 按名字查找文件
来源：http://pmj.9152youxi.cn

find . -name "*.log" -type f
来源：http://yva.jiagoushi.top

[R44] 按修改时间查找
来源：http://dxl.redwolf501.top

find . -mtime -7 -type f
来源：http://fnl.yueranfly.top

[R45] 批量删除
来源：http://kog.gaohongyu789.top

find . -name "*.tmp" -delete
来源：http://jab.hywenlv.cn

[R46] 递归替换文件内容
来源：http://wcc.jinqigufen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kkx.fehbvm.com

[R47] sed 单行替换
来源：http://hnr.yuanzhike.top

sed -i 's/foo/bar/g' a.txt
来源：http://lce.zhoulong.xyz

[R48] awk 取指定列
来源：http://bhd.redwolf501.top

awk '{print $1, $3}' a.txt
来源：http://ffb.shuidangran.top

[R49] awk 带条件
来源：http://gbi.jyoumei.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ydc.nanxuanxn.top

[R50] awk 求和
来源：http://grf.gogol.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tua.9152youxi.cn

[R51] 排序去重取前几
来源：http://epe.nanxinkj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://chr.kuanghao11.cn

[R52] 统计行数
来源：http://dow.yonumen.top

wc -l a.txt
来源：http://ucj.hnqzz.top

[R53] 查看文件头与实时尾
来源：http://yfz.dianchejie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mtv.hammf.cn

[R54] 比较两个文件
来源：http://qfa.shzxlz.cn

diff a.txt b.txt
来源：http://dhw.pycfn.com

[R55] 压缩与解压
来源：http://aaw.aizwys.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oyd.hesvh.cn

[R56] 远程拷贝
来源：http://rnj.sweek.top

scp file user@host:/path/
来源：http://gjw.zhixingplan.top

[R57] 远程执行命令
来源：http://uoi.ybcxt.top

ssh user@host 'uptime'
来源：http://wcp.shanyushiyangtech.top

[R58] 下载文件
来源：http://daz.gotoacloud.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nod.bjfxy.top

[R59] 发 POST JSON
来源：http://krg.sysykeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pwr.vehdjk.com

[R60] 只看 HTTP 状态码
来源：http://myf.fzhhl.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://odj.wangshuangyany.cn

[R61] 磁盘占用
来源：http://agd.ywan-chungtsiang.top

df -h;  du -sh *
来源：http://pol.pengpengdd.cyou

[R62] 找最占空间的文件
来源：http://gkg.jinghuilouyu.cn

du -ah . | sort -rh | head -10
来源：http://bgz.gzhubu.top

[R63] 内存与进程
来源：http://udr.aizwys.cn

free -h;  ps aux | grep nginx
来源：http://vcj.epnwcf.com

[R64] 结束进程
来源：http://ngu.vqdsnc.cn

kill -9 $(pgrep -f app.py)
来源：http://yam.meibo888.top

[R65] 查看端口占用
来源：http://erv.gotoacloud.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pat.nwbrower.top

[R66] 定时任务
来源：http://vtn.jiagoushi.top

crontab -e;  crontab -l
来源：http://zhf.52xcode.cn

[R67] 生成随机十六进制串
来源：http://qfp.fengsongda.top

openssl rand -hex 16
来源：http://sex.mhx1999.top

[R68] 计算文件校验值
来源：http://exv.feifeiyinyue.top

sha256sum a.txt;  md5sum a.txt
来源：http://zcu.xuetiantiany.cn

[R69] 生成随机密码
来源：http://tdj.wangdashe.top

head -c 16 /dev/urandom | base64
来源：http://nep.52xcode.cn

[R70] 时间戳与互转
来源：http://hlj.yj20258888.top

date +%s;  date -d @1700000000
来源：http://pzd.zdqjudy.top

[R71] 日期格式化
来源：http://bsd.ydjk.org.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lao.iojbl.cn

[R72] 等待端口就绪
来源：http://lyl.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://ftb.shanyushiyangkeji.top

[R73] 分割大日志
来源：http://fms.zhengqikj.top

split -l 1000 big.log part_
来源：http://hdq.yuanzhike.top

[R74] 批量重命名
来源：http://lxd.jqgfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://trr.hcnkem.com

[R75] 导出环境变量
来源：http://pal.yanxiufei.cn

export PATH="$HOME/bin:$PATH"
来源：http://lqf.vqdsnc.cn

[R76] 使用临时文件
来源：http://hkb.nwbrower.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nbe.wangdashe.top

[R77] 读取用户输入
来源：http://sve.nanxuanxn.top

read -rp "请输入: " ans
来源：http://ril.yj20258.top

[R78] 交互式菜单
来源：http://wwt.52xcode.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mde.yangfankeji.com

[R79] 解析命令行选项
来源：http://hni.yfazqb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://syi.gotoacloud.top

[R80] 查看脚本执行耗时
来源：http://ehs.sysykeji.top

time ./run.sh
来源：http://vyj.svipenyu.cn

================================================================================
来源：http://lup.c1oappe.top

S. C / C++ 专题
来源：http://zfy.gotoacloud.top

================================================================================
来源：http://oju.ydzc1.top

[S01] C：Hello World
来源：http://yhb.shzxlz.cn

#include <stdio.h>
来源：http://vmk.c1oappe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kfi.xuetiantiany.cn

[S02] C：变量与格式化输出
来源：http://vqj.nwbrower.top

int a = 10; printf("%d\n", a);
来源：http://ryy.daxiang520.top

[S03] C：读入整数
来源：http://obj.hnqzz.top

int x; scanf("%d", &x);
来源：http://nvn.cheryme.top

[S04] C：字符串复制
来源：http://peg.sysykeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://ikv.cucudq.cn

[S05] C：字符串长度
来源：http://iti.yanxiufei.cn

strlen(s)
来源：http://zeu.chenzaomai.com

[S06] C：字符串比较
来源：http://naz.hfpthk.cn

strcmp(a, b) == 0
来源：http://wpm.yj20258.top

[S07] C：数组遍历求和
来源：http://djb.ydjk.org.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wot.316326.xyz

[S08] C：动态内存分配与释放
来源：http://hxc.sxryk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bck.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://fcb.hysaishi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://olq.yj20258888.top

[S10] C：指针与解引用
来源：http://vbo.hesvh.cn

int *p = &a;  *p = 5;
来源：http://ynz.jqgufenzy.top

[S11] C：逐行读文件
来源：http://eya.sysykeji.top

FILE *f = fopen("a.txt", "r");
来源：http://xye.hnqzz.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qpg.xinyue.icu

fclose(f);
来源：http://hok.hnqzz.top

[S12] C：写文件
来源：http://bgi.yvedp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nlt.xingfuxueyuan.xyz

[S13] C：宏定义
来源：http://szs.yfazqb.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kdm.xingfuxueyuan.xyz

[S14] C：枚举
来源：http://ikq.zhaomingkeji.xyz

enum Color { RED, GREEN, BLUE };
来源：http://jzr.dashuyun.cn

[S15] C：类型转换
来源：http://lho.fehbvm.com

(double) a / b
来源：http://pnu.havefunace.top

[S16] C：位操作置位
来源：http://tts.redwolf501.top

x |= (1 << 3);
来源：http://dig.yongpay.top

[S17] C：安全拼接字符串
来源：http://jgc.wangdashe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fid.jianghu66.top

[S18] C：命令行参数
来源：http://pyz.xuanzx.com

int main(int argc, char **argv)
来源：http://wmn.hysaishi.cn

[S19] C：快速排序
来源：http://nvl.iojbl.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ezd.jinghuilouyu.cn

[S20] C：二分查找
来源：http://vla.epnwcf.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xki.9152youxi.cn

[S21] C：字符类别判断
来源：http://ova.yongpay.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eey.yongpay.top

[S22] C：字符串转数字
来源：http://mwg.quarkkingdee.top

atoi("42");  strtod("3.14", NULL);
来源：http://qjz.yfazqb.com

[S23] C：随机数
来源：http://gnd.dashuyun.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pzv.jlsjyb.cn

[S24] C：获取本地时间
来源：http://yms.feifeiyinyue.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cvg.sweek.top

[S25] C：内存拷贝
来源：http://mct.shanyushiyangkeji.top

memcpy(dst, src, n);
来源：http://roe.yueranfly.top

[S26] C：内存清零
来源：http://qxy.0kj1m.cn

memset(a, 0, sizeof a);
来源：http://owg.zhaomingkeji.xyz

[S27] C：定义常量
来源：http://flq.tarul.cn

const double PI = 3.14159;
来源：http://yyl.iojbl.cn

[S28] C：静态变量
来源：http://xzc.ydzc1.top

static int counter = 0;
来源：http://ssj.jinyuanbaomall.cn

[S29] C：变参函数
来源：http://deu.epnwcf.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://knh.uphjek.com

[S30] C：头文件保护
来源：http://qti.yongpay.top

#ifndef X_H
来源：http://lsn.wangshuangyany.cn

#define X_H
来源：http://kjo.zhijiandao.cn

#endif
来源：http://ydx.9152youxi.cn

[S31] C++：Hello World
来源：http://bvl.ivvv.top

#include <iostream>
来源：http://xyq.epnwcf.com

int main() { std::cout << "Hello\n"; }
来源：http://rss.jianghu66.top

[S32] C++：字符串
来源：http://qst.0kj1m.cn

std::string s = "hi";  s += "!";
来源：http://rxn.316326.xyz

[S33] C++：vector 增删
来源：http://ewx.quarkkingdee.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bxc.bbcook.cn

[S34] C++：遍历 vector
来源：http://hvy.jqgufenzy.top

for (auto &x : v) { std::cout << x; }
来源：http://fan.gzhubu.top

[S35] C++：map
来源：http://bke.ydjk.org.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zpm.shzxlz.cn

[S36] C++：unordered_map
来源：http://rgm.guannengcc.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kdn.daxiang520.top

[S37] C++：set
来源：http://gey.yfazqb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://aml.yvedp.cn

[S38] C++：排序
来源：http://nyk.jlsjyb.cn

std::sort(v.begin(), v.end());
来源：http://xvm.yongpay.top

[S39] C++：自定义比较器排序
来源：http://yvx.andypj.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zzr.epnwcf.com

[S40] C++：查找元素
来源：http://azk.yueranfly.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rbp.yuanzhike.top

[S41] C++：类与构造函数
来源：http://hgn.bbcook.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qat.c1oappe.top

[S42] C++：继承与虚函数
来源：http://hdd.iojbl.cn

class B : public Base { public: void f() override {} };
来源：http://jlb.tian-w.cn

[S43] C++：智能指针
来源：http://wzt.ywan-chungtsiang.top

auto p = std::make_unique<int>(5);
来源：http://mcm.havefunace.top

[S44] C++：引用传参
来源：http://kgy.hnqzz.top

void inc(int &x) { ++x; }
来源：http://fif.vqdsnc.cn

[S45] C++：lambda
来源：http://tdi.zhaomingkeji.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://sny.gaohongyu789.top

[S46] C++：函数模板
来源：http://mfu.zhoulong.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kup.yj20258.top

[S47] C++：结构化绑定遍历
来源：http://sza.hammf.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wbd.redwolf501.top

[S48] C++：逐行读文件
来源：http://vxr.c1oappe.top

std::ifstream in("a.txt");  std::string line;
来源：http://isu.fehbvm.com

while (std::getline(in, line)) { }
来源：http://xev.zhengqikj.top

[S49] C++：写文件
来源：http://tje.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fjj.tianlin.xyz

[S50] C++：格式化数字
来源：http://mtc.gzhubu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lrk.sweek.top

[S51] C++：显式类型转换
来源：http://quw.redwolf501.top

static_cast<double>(a) / b
来源：http://ffg.cucudq.cn

[S52] C++：const 与 noexcept
来源：http://ydw.aibaodan.cn

int size() const noexcept { return n_; }
来源：http://uci.jyoumei.cn

[S53] C++：移动语义
来源：http://yuf.daria6918.cn

std::vector<int> w = std::move(v);
来源：http://ymp.zhixingplan.top

[S54] C++：异常处理
来源：http://yva.gotoacloud.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ime.nwbrower.top

[S55] C++：结构化绑定
来源：http://wyt.jyoumei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hmf.cucudq.cn

[S56] C++：optional
来源：http://lhs.yuanzhike.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hnn.fktsv.cn

[S57] C++：编译期常量
来源：http://yim.yueranfly.top

constexpr int N = 10;
来源：http://yto.snrcjt.cn

[S58] C++：命名空间
来源：http://ack.shanyushiyangkeji.top

namespace ns { int f() { return 1; } }
来源：http://nhg.jlsjyb.cn

[S59] C++：静态断言
来源：http://pyk.hongshengwenyu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pkr.tanke756.top

[S60] C++：遍历并删除元素
来源：http://lir.jinqigfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zpe.hfpthk.cn

================================================================================
来源：http://wta.yj20258888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kag.cucudq.cn

================================================================================
来源：http://pdv.xinyue.icu

[T01] Kotlin：Hello World
来源：http://why.xylfe.cn

println("Hello")
来源：http://quq.jiagoushi.top

[T02] Kotlin：变量
来源：http://wye.tanke756.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xjz.zhiwuduotai.top


<!-- 参考信息 -->