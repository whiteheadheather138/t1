代发 wailian999

set -euo pipefail
来源：http://ywm.jianghu66.top

[R02] 变量赋值与使用
来源：http://suv.shuidangran.top

name="Tom"; echo "$name"
来源：http://gxi.smart0.xyz

[R03] 只读变量
来源：http://mxt.daxiang520.top

readonly PI=3.14
来源：http://sry.bjfxy.top

[R04] 位置参数
来源：http://xch.hfpthk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oyc.yj20258888.top

[R05] 参数默认值
来源：http://awb.hywenlv.cn

name="${1:-default}"
来源：http://zie.meibo888.top

[R06] 判断命令是否存在
来源：http://pvq.yonumen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://llu.hnqzz.top

[R07] if 判断文件
来源：http://qyy.xingfuxueyuan.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qll.tarul.cn

[R08] 数值比较
来源：http://nah.zycfv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uwr.gogol.net.cn

[R09] 字符串比较
来源：http://mdf.gogol.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xvw.9152youxi.cn

[R10] 正则匹配
来源：http://fty.sweek.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uwz.yvedp.cn

[R11] case 多分支
来源：http://ynt.fehbvm.com

case "$1" in
来源：http://btj.xingfuxueyuan.xyz

start) echo "启动" ;;
来源：http://jpp.hysaishi.cn

stop)  echo "停止" ;;
来源：http://gya.mhx1999.top

*)     echo "未知命令" ;;
来源：http://buq.cucudq.cn

esac
来源：http://tzz.jqgfzy.top

[R12] for 遍历文件
来源：http://yxi.jianghu66.top

for f in *.txt; do echo "$f"; done
来源：http://aqu.shuidangran.top

[R13] for 计数循环
来源：http://wbw.yj202588.top

for i in {1..10}; do echo "$i"; done
来源：http://vqc.ydzc1.top

[R14] C 风格 for
来源：http://nja.c1oappe.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oft.bbcook.cn

[R15] while 逐行读文件
来源：http://elz.9152youxi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yev.zycfv.cn

[R16] until 等待条件
来源：http://ymp.chenlongwang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yvg.meibo888.top

[R17] 数组定义与取值
来源：http://wqb.shzxlz.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bre.zhongyouzk.top

[R18] 遍历数组
来源：http://fys.zycfv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://muz.yj20258.top

[R19] 数组长度
来源：http://png.sweek.top

echo "${#arr[@]}"
来源：http://bvp.jqgfzy.top

[R20] 关联数组（字典）
来源：http://nwg.chenjidiqi.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bkf.yueranfly.top

[R21] 字符串长度
来源：http://rbi.zdqjudy.top

echo "${#s}"
来源：http://iri.uphjek.com

[R22] 截取子串
来源：http://jus.zhongyouzk.top

echo "${s:0:5}"
来源：http://kpn.jlsjyb.cn

[R23] 字符串替换
来源：http://ljj.shuidangran.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ylz.xziqi.cn

[R24] 大小写转换
来源：http://xfh.fzhhl.top

echo "${s^^}"; echo "${s,,}"
来源：http://mvx.redwolf501.top

[R25] 去后缀 / 去前缀
来源：http://htt.cucudq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://stq.gzhubu.top

[R26] 命令替换
来源：http://ida.shuidangran.top

now=$(date +%F); echo "$now"
来源：http://dxy.xinyue.icu

[R27] 算术展开
来源：http://atq.hnxiangtu.top

echo $((1 + 2 * 3))
来源：http://jut.zdbjq.cn

[R28] 浮点运算
来源：http://nua.sysykeji.top

echo "scale=2; 10/3" | bc
来源：http://riu.wangshuangyany.cn

[R29] 定义函数
来源：http://ezr.xinyue.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pqt.xinyue.icu

[R30] 函数返回状态码
来源：http://qfk.zhiwuduotai.top

f() { return 0; }; f || echo "失败了"
来源：http://avi.ydzc1.top

[R31] 局部变量
来源：http://daw.jyoumei.cn

f() { local x=1; echo "$x"; }
来源：http://xao.cqqwz.cn

[R32] 参数个数校验
来源：http://psm.nanxuanxn.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ent.yj20258888.top

[R33] 捕获错误并提示行号
来源：http://rdu.316326.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wvk.uphjek.com

[R34] 退出时清理
来源：http://pba.guowangkeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://hdl.iojbl.cn

[R35] 后台执行并等待
来源：http://gjm.pengpengdd.cyou

sleep 5 & pid=$!; wait "$pid"
来源：http://ssn.jinqigfzy.top

[R36] 并发执行多个任务
来源：http://hiv.jqgufenzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jdw.cucudq.cn

[R37] 把输出赋给变量
来源：http://ylp.yangfankeji.com

files=$(ls -1)
来源：http://ieu.gogol.net.cn

[R38] 管道串联
来源：http://hov.haohaochexian.top

cat a.txt | grep -i error | wc -l
来源：http://gpx.hysaishi.cn

[R39] 重定向标准输出与错误
来源：http://qqr.nanxinkj.top

cmd > out.log 2>&1
来源：http://hux.316326.xyz

[R40] 追加写日志
来源：http://ngm.havefunace.top

echo "log" >> out.log
来源：http://vlg.hcnkem.com

[R41] 丢弃输出
来源：http://pfd.zdbjq.cn

cmd >/dev/null 2>&1
来源：http://xaz.cheryme.top

[R42] 输入重定向
来源：http://zpo.hysaishi.cn

wc -l < a.txt
来源：http://vsi.pycfn.com

[R43] 按名字查找文件
来源：http://rso.xingfuxueyuan.xyz

find . -name "*.log" -type f
来源：http://ade.jianghu66.top

[R44] 按修改时间查找
来源：http://sxk.haohaochexian.top

find . -mtime -7 -type f
来源：http://nla.jqgufenzy.top

[R45] 批量删除
来源：http://jnr.zhoulong.xyz

find . -name "*.tmp" -delete
来源：http://lek.vqdsnc.cn

[R46] 递归替换文件内容
来源：http://rst.ivvv.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dxe.jinyuanbaomall.cn

[R47] sed 单行替换
来源：http://mbu.zhixingplan.top

sed -i 's/foo/bar/g' a.txt
来源：http://dho.zdbjq.cn

[R48] awk 取指定列
来源：http://jvz.zhengqikj.top

awk '{print $1, $3}' a.txt
来源：http://ebb.jinqigufen.top

[R49] awk 带条件
来源：http://buq.ywan-chungtsiang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ixb.zhiwuduotai.top

[R50] awk 求和
来源：http://ayc.kuanghao11.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ads.shzxlz.cn

[R51] 排序去重取前几
来源：http://ekp.zhijiandao.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://quv.ywan-chungtsiang.top

[R52] 统计行数
来源：http://pmr.zhixingplan.top

wc -l a.txt
来源：http://esz.sweek.top

[R53] 查看文件头与实时尾
来源：http://bro.yongpay.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gha.ydjk.org.cn

[R54] 比较两个文件
来源：http://mas.nanxinkj.top

diff a.txt b.txt
来源：http://apg.shangyingyoupin.top

[R55] 压缩与解压
来源：http://mjt.hcnkem.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nzy.cheryme.top

[R56] 远程拷贝
来源：http://amv.gzhubu.top

scp file user@host:/path/
来源：http://maz.sweek.top

[R57] 远程执行命令
来源：http://iwx.birdmap.top

ssh user@host 'uptime'
来源：http://hui.yangfankeji.com

[R58] 下载文件
来源：http://dbm.aibaodan.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xkc.hesvh.cn

[R59] 发 POST JSON
来源：http://mkf.zhoulong.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ccu.jiagoushi.top

[R60] 只看 HTTP 状态码
来源：http://puc.xinyue.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zcy.daria6918.cn

[R61] 磁盘占用
来源：http://djh.nwbrower.top

df -h;  du -sh *
来源：http://gnv.pengpengdd.cyou

[R62] 找最占空间的文件
来源：http://owr.xinyue.icu

du -ah . | sort -rh | head -10
来源：http://how.daria6918.cn

[R63] 内存与进程
来源：http://gwr.hnqzz.top

free -h;  ps aux | grep nginx
来源：http://exb.jinghuilouyu.cn

[R64] 结束进程
来源：http://toq.hywenlv.cn

kill -9 $(pgrep -f app.py)
来源：http://mix.hnxiangtu.top

[R65] 查看端口占用
来源：http://qsr.gotoacloud.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://msf.sxryk.cn

[R66] 定时任务
来源：http://acy.jqgufenzy.top

crontab -e;  crontab -l
来源：http://ect.aibaodan.cn

[R67] 生成随机十六进制串
来源：http://bzu.jinghuilouyu.cn

openssl rand -hex 16
来源：http://oim.mhx1999.top

[R68] 计算文件校验值
来源：http://esh.ehwqpu.com

sha256sum a.txt;  md5sum a.txt
来源：http://zqw.yj20258.top

[R69] 生成随机密码
来源：http://ldp.0kj1m.cn

head -c 16 /dev/urandom | base64
来源：http://uxe.pycfn.com

[R70] 时间戳与互转
来源：http://ltc.gaohongyu789.top

date +%s;  date -d @1700000000
来源：http://myf.cheryme.top

[R71] 日期格式化
来源：http://juj.daxiang520.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dfk.gzhubu.top

[R72] 等待端口就绪
来源：http://sfn.daria6918.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://eor.guannengcc.top

[R73] 分割大日志
来源：http://tjp.jinghuilouyu.cn

split -l 1000 big.log part_
来源：http://lha.gotoacloud.top

[R74] 批量重命名
来源：http://hbo.feifeiyinyue.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aab.vehdjk.com

[R75] 导出环境变量
来源：http://yuc.cashguo.top

export PATH="$HOME/bin:$PATH"
来源：http://bxl.xinyue.icu

[R76] 使用临时文件
来源：http://xxg.epnwcf.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://stn.aibaodan.cn

[R77] 读取用户输入
来源：http://mqm.vqdsnc.cn

read -rp "请输入: " ans
来源：http://gtu.wangdashe.top

[R78] 交互式菜单
来源：http://oqm.iojbl.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://irs.daria6918.cn

[R79] 解析命令行选项
来源：http://mow.kuanghao11.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xsj.xylfe.cn

[R80] 查看脚本执行耗时
来源：http://eeo.c1oappe.top

time ./run.sh
来源：http://rve.wangshuangyany.cn

================================================================================
来源：http://cij.jqgufenzy.top

S. C / C++ 专题
来源：http://mlp.cucudq.cn

================================================================================
来源：http://fqk.dianchejie.cn

[S01] C：Hello World
来源：http://odz.sysykeji.top

#include <stdio.h>
来源：http://fdm.yvedp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bbl.hnqzz.top

[S02] C：变量与格式化输出
来源：http://coi.cucudq.cn

int a = 10; printf("%d\n", a);
来源：http://zsd.zdbjq.cn

[S03] C：读入整数
来源：http://twa.fehbvm.com

int x; scanf("%d", &x);
来源：http://wga.yonumen.top

[S04] C：字符串复制
来源：http://jqw.hnxiangtu.top

char dst[32]; strcpy(dst, "hi");
来源：http://nby.chenzaomai.com

[S05] C：字符串长度
来源：http://eom.feifeiyinyue.top

strlen(s)
来源：http://dvy.iojbl.cn

[S06] C：字符串比较
来源：http://jdc.dianchejie.cn

strcmp(a, b) == 0
来源：http://zeo.9152youxi.cn

[S07] C：数组遍历求和
来源：http://bky.vehdjk.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ktg.shanyushiyangtech.top

[S08] C：动态内存分配与释放
来源：http://dtx.jiagoushi.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ljj.gotoacloud.top

[S09] C：结构体定义与初始化
来源：http://wkr.bjfxy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wsz.jianghu66.top

[S10] C：指针与解引用
来源：http://koa.sxryk.cn

int *p = &a;  *p = 5;
来源：http://pel.mhx1999.top

[S11] C：逐行读文件
来源：http://nfo.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://los.chenzaomai.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://rxx.cheryme.top

fclose(f);
来源：http://omy.sxryk.cn

[S12] C：写文件
来源：http://mwk.jianghu66.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qwv.zhoulong.xyz

[S13] C：宏定义
来源：http://oxr.redwolf501.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kli.hnxiangtu.top

[S14] C：枚举
来源：http://gym.xinyue.icu

enum Color { RED, GREEN, BLUE };
来源：http://pci.yj20258.top

[S15] C：类型转换
来源：http://tcv.ivvv.top

(double) a / b
来源：http://vbc.zhengqikj.top

[S16] C：位操作置位
来源：http://djn.yvedp.cn

x |= (1 << 3);
来源：http://zcv.bjfxy.top

[S17] C：安全拼接字符串
来源：http://uxb.nanxuanxn.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lcf.yangfankeji.com

[S18] C：命令行参数
来源：http://ncc.yonumen.top

int main(int argc, char **argv)
来源：http://jva.hcnkem.com

[S19] C：快速排序
来源：http://vbx.jqgufenzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://zbr.smart0.xyz

[S20] C：二分查找
来源：http://zor.xuanzx.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lio.c1oappe.top

[S21] C：字符类别判断
来源：http://vox.tarul.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xhh.52xcode.cn

[S22] C：字符串转数字
来源：http://vby.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://vnr.0kj1m.cn

[S23] C：随机数
来源：http://gvh.hnxiangtu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xjd.yuxming.cn

[S24] C：获取本地时间
来源：http://xhf.gotoacloud.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lhr.shangyingyoupin.top

[S25] C：内存拷贝
来源：http://pyt.gogol.net.cn

memcpy(dst, src, n);
来源：http://zca.hysaishi.cn

[S26] C：内存清零
来源：http://ktb.redwolf501.top

memset(a, 0, sizeof a);
来源：http://aoi.sufxvd.cn

[S27] C：定义常量
来源：http://kib.nanxuanxn.top

const double PI = 3.14159;
来源：http://vkq.guannengcc.top

[S28] C：静态变量
来源：http://nsz.316326.xyz

static int counter = 0;
来源：http://pat.zycfv.cn

[S29] C：变参函数
来源：http://bhy.shuidangran.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://trc.c1oappe.top

[S30] C：头文件保护
来源：http://kpf.jinyuanbaomall.cn

#ifndef X_H
来源：http://wia.jiagoushi.top

#define X_H
来源：http://vch.316326.xyz

#endif
来源：http://bxq.sysykeji.top

[S31] C++：Hello World
来源：http://nxl.ivvv.top

#include <iostream>
来源：http://zzc.bjfxy.top

int main() { std::cout << "Hello\n"; }
来源：http://pfw.zhongyouzk.top

[S32] C++：字符串
来源：http://fcl.pengpengdd.cyou

std::string s = "hi";  s += "!";
来源：http://nri.aizwys.cn

[S33] C++：vector 增删
来源：http://vcj.jyoumei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mkc.fengsongda.top

[S34] C++：遍历 vector
来源：http://cyj.xuanzx.com

for (auto &x : v) { std::cout << x; }
来源：http://wee.xziqi.cn

[S35] C++：map
来源：http://rku.shzxlz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gyq.zhiwuduotai.top

[S36] C++：unordered_map
来源：http://snn.vqdsnc.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ajs.gaohongyu789.top

[S37] C++：set
来源：http://vdv.aibaodan.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qsc.shuidangran.top

[S38] C++：排序
来源：http://dnw.yangfankeji.com

std::sort(v.begin(), v.end());
来源：http://qvi.jinghuilouyu.cn

[S39] C++：自定义比较器排序
来源：http://zor.ivvv.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nnk.yvedp.cn

[S40] C++：查找元素
来源：http://frd.dashuyun.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ipq.0kj1m.cn

[S41] C++：类与构造函数
来源：http://cbr.svipenyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tbp.daxiang520.top

[S42] C++：继承与虚函数
来源：http://rug.ydjk.org.cn

class B : public Base { public: void f() override {} };
来源：http://irw.gotoacloud.top

[S43] C++：智能指针
来源：http://vcf.fengsongda.top

auto p = std::make_unique<int>(5);
来源：http://gdi.zhongyouzk.top

[S44] C++：引用传参
来源：http://irf.52xcode.cn

void inc(int &x) { ++x; }
来源：http://uld.nwbrower.top

[S45] C++：lambda
来源：http://qjw.chenlongwang.top

auto add = [](int a, int b) { return a + b; };
来源：http://rlc.chenlongwang.top

[S46] C++：函数模板
来源：http://wya.cdnleiting.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nde.yonumen.top

[S47] C++：结构化绑定遍历
来源：http://krv.fanxiaobao.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gms.hysaishi.cn

[S48] C++：逐行读文件
来源：http://jsd.xylfe.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rrk.ppjwa.cn

while (std::getline(in, line)) { }
来源：http://qke.svipenyu.cn

[S49] C++：写文件
来源：http://bpq.zhengqikj.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pwf.yueranfly.top

[S50] C++：格式化数字
来源：http://qac.chenzaomai.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wpm.epnwcf.com

[S51] C++：显式类型转换
来源：http://tya.wangshuangyany.cn

static_cast<double>(a) / b
来源：http://iwx.ehwqpu.com

[S52] C++：const 与 noexcept
来源：http://ynx.zhijiandao.cn

int size() const noexcept { return n_; }
来源：http://efn.zdqjudy.top

[S53] C++：移动语义
来源：http://ifb.guowangkeji.top

std::vector<int> w = std::move(v);
来源：http://tjv.zhijiandao.cn

[S54] C++：异常处理
来源：http://uao.xylfe.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ine.chenjidiqi.icu

[S55] C++：结构化绑定
来源：http://abs.vehdjk.com

auto [a, b] = std::make_pair(1, 2);
来源：http://owk.chenjidiqi.icu

[S56] C++：optional
来源：http://saa.zhoulong.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ubt.xziqi.cn

[S57] C++：编译期常量
来源：http://quw.fktsv.cn

constexpr int N = 10;
来源：http://dlf.shanyushiyangkeji.top

[S58] C++：命名空间
来源：http://gjr.xinyue.icu

namespace ns { int f() { return 1; } }
来源：http://lnh.yonumen.top

[S59] C++：静态断言
来源：http://tjk.sjlbkw.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bac.9152youxi.cn

[S60] C++：遍历并删除元素
来源：http://zrd.hysaishi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://acy.feifeiyinyue.top

================================================================================
来源：http://uxu.tian-w.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rls.daria6918.cn

================================================================================
来源：http://wbo.hywenlv.cn

[T01] Kotlin：Hello World
来源：http://ojj.hammf.cn

println("Hello")
来源：http://gfp.cqqwz.cn

[T02] Kotlin：变量
来源：http://zus.ybcxt.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://snl.ydjk.org.cn


<!-- 参考信息 -->