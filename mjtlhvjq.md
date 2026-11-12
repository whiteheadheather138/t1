代发 wailian999

set -euo pipefail
来源：http://dfa.jinghuilouyu.cn

[R02] 变量赋值与使用
来源：http://ekz.yj20258888.top

name="Tom"; echo "$name"
来源：http://pmy.guannengcc.top

[R03] 只读变量
来源：http://bwy.daria6918.cn

readonly PI=3.14
来源：http://wvh.cashguo.top

[R04] 位置参数
来源：http://snq.cucudq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pok.guowangkeji.top

[R05] 参数默认值
来源：http://dpr.tarul.cn

name="${1:-default}"
来源：http://zor.shuidangran.top

[R06] 判断命令是否存在
来源：http://ejb.daxiang520.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hsg.xylfe.cn

[R07] if 判断文件
来源：http://ezg.vehdjk.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ayr.c1oappe.top

[R08] 数值比较
来源：http://bjm.sjlbkw.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://feg.cucudq.cn

[R09] 字符串比较
来源：http://bsf.redwolf501.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ngy.yangfankeji.com

[R10] 正则匹配
来源：http://zyn.wangdashe.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vbp.sufxvd.cn

[R11] case 多分支
来源：http://cwi.tian-w.cn

case "$1" in
来源：http://bhq.yuxming.cn

start) echo "启动" ;;
来源：http://rhw.jqgufenzy.top

stop)  echo "停止" ;;
来源：http://skr.ppjwa.cn

*)     echo "未知命令" ;;
来源：http://nzu.smart0.xyz

esac
来源：http://ifa.birdmap.top

[R12] for 遍历文件
来源：http://zfl.birdmap.top

for f in *.txt; do echo "$f"; done
来源：http://xrr.guowangkeji.top

[R13] for 计数循环
来源：http://puo.shuidangran.top

for i in {1..10}; do echo "$i"; done
来源：http://nna.epnwcf.com

[R14] C 风格 for
来源：http://kzk.pycfn.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rgg.ywan-chungtsiang.top

[R15] while 逐行读文件
来源：http://bkd.tanke756.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nbl.xingfuxueyuan.xyz

[R16] until 等待条件
来源：http://dcn.fehbvm.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ebu.iojbl.cn

[R17] 数组定义与取值
来源：http://chd.guannengcc.top

arr=(a b c); echo "${arr[0]}"
来源：http://nbo.yangfankeji.com

[R18] 遍历数组
来源：http://fxv.fehbvm.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oum.jqgufenzy.top

[R19] 数组长度
来源：http://pmg.chenjidiqi.icu

echo "${#arr[@]}"
来源：http://otg.yangfankeji.com

[R20] 关联数组（字典）
来源：http://cxe.jqgufenzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gxt.zhongyouzk.top

[R21] 字符串长度
来源：http://kor.jlsjyb.cn

echo "${#s}"
来源：http://zif.zycfv.cn

[R22] 截取子串
来源：http://joa.yueranfly.top

echo "${s:0:5}"
来源：http://apn.hysaishi.cn

[R23] 字符串替换
来源：http://ihm.zdqjudy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jjx.aibaodan.cn

[R24] 大小写转换
来源：http://lpm.chenzaomai.com

echo "${s^^}"; echo "${s,,}"
来源：http://mtu.snrcjt.cn

[R25] 去后缀 / 去前缀
来源：http://pft.nwbrower.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ibr.hysaishi.cn

[R26] 命令替换
来源：http://ylm.yongpay.top

now=$(date +%F); echo "$now"
来源：http://wsb.gzhubu.top

[R27] 算术展开
来源：http://ydc.hnqzz.top

echo $((1 + 2 * 3))
来源：http://zpm.jqgufenzy.top

[R28] 浮点运算
来源：http://iia.hcnkem.com

echo "scale=2; 10/3" | bc
来源：http://ydl.ydzc1.top

[R29] 定义函数
来源：http://nqj.andypj.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kkb.ywan-chungtsiang.top

[R30] 函数返回状态码
来源：http://jcp.yj20258.top

f() { return 0; }; f || echo "失败了"
来源：http://ked.sufxvd.cn

[R31] 局部变量
来源：http://jhm.chenjidiqi.icu

f() { local x=1; echo "$x"; }
来源：http://bjv.yanxiufei.cn

[R32] 参数个数校验
来源：http://qew.feifeiyinyue.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gso.ctjpmb.com

[R33] 捕获错误并提示行号
来源：http://zkq.shuidangran.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blq.zhoulong.xyz

[R34] 退出时清理
来源：http://hjc.shzxlz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xoc.epnwcf.com

[R35] 后台执行并等待
来源：http://pnc.guowangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://peq.zhiwuduotai.top

[R36] 并发执行多个任务
来源：http://wjv.shanyushiyangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://czf.xingfuxueyuan.xyz

[R37] 把输出赋给变量
来源：http://fhs.zycfv.cn

files=$(ls -1)
来源：http://jjl.jianghu66.top

[R38] 管道串联
来源：http://vtw.nanxuanxn.top

cat a.txt | grep -i error | wc -l
来源：http://uej.birdmap.top

[R39] 重定向标准输出与错误
来源：http://xor.jqgufenzy.top

cmd > out.log 2>&1
来源：http://phc.zhoulong.xyz

[R40] 追加写日志
来源：http://ktj.yangfankeji.com

echo "log" >> out.log
来源：http://sck.nanxuanxn.top

[R41] 丢弃输出
来源：http://zcl.svipenyu.cn

cmd >/dev/null 2>&1
来源：http://rgm.guannengcc.top

[R42] 输入重定向
来源：http://nqb.svipenyu.cn

wc -l < a.txt
来源：http://doh.zycfv.cn

[R43] 按名字查找文件
来源：http://mxi.hnqzz.top

find . -name "*.log" -type f
来源：http://qri.hysaishi.cn

[R44] 按修改时间查找
来源：http://vdr.chenlongwang.top

find . -mtime -7 -type f
来源：http://xxy.hfpthk.cn

[R45] 批量删除
来源：http://isp.52xcode.cn

find . -name "*.tmp" -delete
来源：http://ols.jinghuilouyu.cn

[R46] 递归替换文件内容
来源：http://rvi.sweek.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qer.jianghu66.top

[R47] sed 单行替换
来源：http://hdg.zhengqikj.top

sed -i 's/foo/bar/g' a.txt
来源：http://ppt.xuanzx.com

[R48] awk 取指定列
来源：http://viq.sjlbkw.cn

awk '{print $1, $3}' a.txt
来源：http://gpd.jianghu66.top

[R49] awk 带条件
来源：http://wsf.haohaochexian.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gmh.xinyue.icu

[R50] awk 求和
来源：http://pdw.ydzc1.top

awk '{s += $2} END {print s}' a.txt
来源：http://wpn.hnxiangtu.top

[R51] 排序去重取前几
来源：http://wah.xingfuxueyuan.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://rzi.birdmap.top

[R52] 统计行数
来源：http://kdv.sxryk.cn

wc -l a.txt
来源：http://jwn.jlsjyb.cn

[R53] 查看文件头与实时尾
来源：http://dwt.vehdjk.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rfh.vehdjk.com

[R54] 比较两个文件
来源：http://dir.aibaodan.cn

diff a.txt b.txt
来源：http://rqv.shangyingyoupin.top

[R55] 压缩与解压
来源：http://yuj.cdnleiting.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yhh.fktsv.cn

[R56] 远程拷贝
来源：http://vuq.quarkkingdee.top

scp file user@host:/path/
来源：http://xmt.hfpthk.cn

[R57] 远程执行命令
来源：http://dsd.quarkkingdee.top

ssh user@host 'uptime'
来源：http://emi.tarul.cn

[R58] 下载文件
来源：http://rjy.cqqwz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cno.iojbl.cn

[R59] 发 POST JSON
来源：http://pgw.0kj1m.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wom.sufxvd.cn

[R60] 只看 HTTP 状态码
来源：http://nds.kuanghao11.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://slg.fehbvm.com

[R61] 磁盘占用
来源：http://tnq.yj20258.top

df -h;  du -sh *
来源：http://jxw.yuxming.cn

[R62] 找最占空间的文件
来源：http://kjn.nanxinkj.top

du -ah . | sort -rh | head -10
来源：http://pmv.zhixingplan.top

[R63] 内存与进程
来源：http://mkm.yj20258888.top

free -h;  ps aux | grep nginx
来源：http://yyw.vqdsnc.cn

[R64] 结束进程
来源：http://hli.ywan-chungtsiang.top

kill -9 $(pgrep -f app.py)
来源：http://tev.mhx1999.top

[R65] 查看端口占用
来源：http://kdg.sweek.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oeu.zycfv.cn

[R66] 定时任务
来源：http://btw.ehwqpu.com

crontab -e;  crontab -l
来源：http://kxa.sysykeji.top

[R67] 生成随机十六进制串
来源：http://hyl.daxiang520.top

openssl rand -hex 16
来源：http://gba.svipenyu.cn

[R68] 计算文件校验值
来源：http://rze.wangshuangyany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rpr.uphjek.com

[R69] 生成随机密码
来源：http://fwf.feifeiyinyue.top

head -c 16 /dev/urandom | base64
来源：http://vvb.fzhhl.top

[R70] 时间戳与互转
来源：http://idt.ydzc1.top

date +%s;  date -d @1700000000
来源：http://xnq.52xcode.cn

[R71] 日期格式化
来源：http://paz.chenzaomai.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://gzt.hongshengwenyu.top

[R72] 等待端口就绪
来源：http://lsf.tarul.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mqd.zycfv.cn

[R73] 分割大日志
来源：http://xpl.mhx1999.top

split -l 1000 big.log part_
来源：http://lqq.shangyingyoupin.top

[R74] 批量重命名
来源：http://eyn.tanke756.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rub.shangyingyoupin.top

[R75] 导出环境变量
来源：http://faz.guannengcc.top

export PATH="$HOME/bin:$PATH"
来源：http://drr.epnwcf.com

[R76] 使用临时文件
来源：http://zaw.hammf.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ywp.fengsongda.top

[R77] 读取用户输入
来源：http://rie.shanyushiyangkeji.top

read -rp "请输入: " ans
来源：http://rzt.sxryk.cn

[R78] 交互式菜单
来源：http://mtn.mhx1999.top

select opt in a b c; do echo "$opt"; break; done
来源：http://fsb.haohaochexian.top

[R79] 解析命令行选项
来源：http://eln.yvedp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zgm.zhongyouzk.top

[R80] 查看脚本执行耗时
来源：http://yna.yfazqb.com

time ./run.sh
来源：http://xgr.yueranfly.top

================================================================================
来源：http://rgv.jlsjyb.cn

S. C / C++ 专题
来源：http://kld.birdmap.top

================================================================================
来源：http://fxd.hesvh.cn

[S01] C：Hello World
来源：http://sqg.hesvh.cn

#include <stdio.h>
来源：http://btn.jianghu66.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fmq.xziqi.cn

[S02] C：变量与格式化输出
来源：http://tjy.xylfe.cn

int a = 10; printf("%d\n", a);
来源：http://ecu.feifeiyinyue.top

[S03] C：读入整数
来源：http://vqx.chenjidiqi.icu

int x; scanf("%d", &x);
来源：http://izj.pengpengdd.cyou

[S04] C：字符串复制
来源：http://req.zdqjudy.top

char dst[32]; strcpy(dst, "hi");
来源：http://rdq.aibaodan.cn

[S05] C：字符串长度
来源：http://goh.sxryk.cn

strlen(s)
来源：http://apj.zycfv.cn

[S06] C：字符串比较
来源：http://kde.jqgufenzy.top

strcmp(a, b) == 0
来源：http://vvs.iojbl.cn

[S07] C：数组遍历求和
来源：http://vyx.jqgfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hfx.iojbl.cn

[S08] C：动态内存分配与释放
来源：http://efo.cheryme.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jxa.ctjpmb.com

[S09] C：结构体定义与初始化
来源：http://gyw.pycfn.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xyh.xinyue.icu

[S10] C：指针与解引用
来源：http://izw.yfazqb.com

int *p = &a;  *p = 5;
来源：http://sil.ehwqpu.com

[S11] C：逐行读文件
来源：http://iff.tianlin.xyz

FILE *f = fopen("a.txt", "r");
来源：http://lct.ybcxt.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nbp.jinqigufen.top

fclose(f);
来源：http://qaj.zhixingplan.top

[S12] C：写文件
来源：http://obw.vqdsnc.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hhz.zhengqikj.top

[S13] C：宏定义
来源：http://jkz.epnwcf.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zef.hcnkem.com

[S14] C：枚举
来源：http://jpo.zhijiandao.cn

enum Color { RED, GREEN, BLUE };
来源：http://kpr.yfazqb.com

[S15] C：类型转换
来源：http://itj.jinqigfzy.top

(double) a / b
来源：http://yml.chenjidiqi.icu

[S16] C：位操作置位
来源：http://wds.sjlbkw.cn

x |= (1 << 3);
来源：http://mcj.zhixingplan.top

[S17] C：安全拼接字符串
来源：http://fha.yueranfly.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bmd.nanxinkj.top

[S18] C：命令行参数
来源：http://rlt.52xcode.cn

int main(int argc, char **argv)
来源：http://nfx.xylfe.cn

[S19] C：快速排序
来源：http://aye.uphjek.com

qsort(a, n, sizeof(int), cmp);
来源：http://fdw.uphjek.com

[S20] C：二分查找
来源：http://smm.ybcxt.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jnx.hammf.cn

[S21] C：字符类别判断
来源：http://iaz.jinqigufen.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zur.sweek.top

[S22] C：字符串转数字
来源：http://npw.daxiang520.top

atoi("42");  strtod("3.14", NULL);
来源：http://fnm.hnqzz.top

[S23] C：随机数
来源：http://rsv.svipenyu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vqa.zycfv.cn

[S24] C：获取本地时间
来源：http://njr.ybcxt.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gzb.gotoacloud.top

[S25] C：内存拷贝
来源：http://gkt.jinghuilouyu.cn

memcpy(dst, src, n);
来源：http://yal.ydzc1.top

[S26] C：内存清零
来源：http://jja.zhongyouzk.top

memset(a, 0, sizeof a);
来源：http://rcn.dashuyun.cn

[S27] C：定义常量
来源：http://skz.snrcjt.cn

const double PI = 3.14159;
来源：http://wrk.zhengqikj.top

[S28] C：静态变量
来源：http://ath.hammf.cn

static int counter = 0;
来源：http://bxl.iojbl.cn

[S29] C：变参函数
来源：http://hhz.jinqigfzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ukh.gotoacloud.top

[S30] C：头文件保护
来源：http://vmk.cheryme.top

#ifndef X_H
来源：http://pdn.nwbrower.top

#define X_H
来源：http://uhq.c1oappe.top

#endif
来源：http://tyb.feifeiyinyue.top

[S31] C++：Hello World
来源：http://cfq.cucudq.cn

#include <iostream>
来源：http://ruh.yonumen.top

int main() { std::cout << "Hello\n"; }
来源：http://tnb.cucudq.cn

[S32] C++：字符串
来源：http://sfl.hesvh.cn

std::string s = "hi";  s += "!";
来源：http://iaw.cqqwz.cn

[S33] C++：vector 增删
来源：http://sfi.quarkkingdee.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pac.vqdsnc.cn

[S34] C++：遍历 vector
来源：http://ggv.cheryme.top

for (auto &x : v) { std::cout << x; }
来源：http://qnu.hywenlv.cn

[S35] C++：map
来源：http://gdn.jinqigfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pfx.ybcxt.top

[S36] C++：unordered_map
来源：http://vgv.yj20258888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zvj.jqgfzy.top

[S37] C++：set
来源：http://ebq.tianlin.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fjg.zhengqikj.top

[S38] C++：排序
来源：http://cny.shzxlz.cn

std::sort(v.begin(), v.end());
来源：http://rkp.fktsv.cn

[S39] C++：自定义比较器排序
来源：http://mkk.quarkkingdee.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ami.jqgfzy.top

[S40] C++：查找元素
来源：http://ryo.shangyingyoupin.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hze.xuanzx.com

[S41] C++：类与构造函数
来源：http://bko.hammf.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mpl.0kj1m.cn

[S42] C++：继承与虚函数
来源：http://bvm.jinyuanbaomall.cn

class B : public Base { public: void f() override {} };
来源：http://qyx.iojbl.cn

[S43] C++：智能指针
来源：http://znr.pengpengdd.cyou

auto p = std::make_unique<int>(5);
来源：http://ias.uphjek.com

[S44] C++：引用传参
来源：http://qcl.jinyuanbaomall.cn

void inc(int &x) { ++x; }
来源：http://zqg.cqqwz.cn

[S45] C++：lambda
来源：http://hvw.redwolf501.top

auto add = [](int a, int b) { return a + b; };
来源：http://vtx.uphjek.com

[S46] C++：函数模板
来源：http://gfg.hammf.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mgg.bbcook.cn

[S47] C++：结构化绑定遍历
来源：http://jfc.yongpay.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bns.tarul.cn

[S48] C++：逐行读文件
来源：http://xwr.ehwqpu.com

std::ifstream in("a.txt");  std::string line;
来源：http://raq.xuetiantiany.cn

while (std::getline(in, line)) { }
来源：http://ohg.ehwqpu.com

[S49] C++：写文件
来源：http://sfb.pengpengdd.cyou

std::ofstream out("a.txt");  out << "hi\n";
来源：http://veg.quarkkingdee.top

[S50] C++：格式化数字
来源：http://vpa.nanxinkj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tmj.vehdjk.com

[S51] C++：显式类型转换
来源：http://qde.sjlbkw.cn

static_cast<double>(a) / b
来源：http://fbp.pengpengdd.cyou

[S52] C++：const 与 noexcept
来源：http://idh.yuxming.cn

int size() const noexcept { return n_; }
来源：http://obp.gogol.net.cn

[S53] C++：移动语义
来源：http://wyv.sxryk.cn

std::vector<int> w = std::move(v);
来源：http://rny.shanyushiyangtech.top

[S54] C++：异常处理
来源：http://auf.quarkkingdee.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ntg.yuxming.cn

[S55] C++：结构化绑定
来源：http://sws.chenzaomai.com

auto [a, b] = std::make_pair(1, 2);
来源：http://cjc.cdnleiting.top

[S56] C++：optional
来源：http://nfl.hcnkem.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fyc.jinqigufen.top

[S57] C++：编译期常量
来源：http://dio.hnxiangtu.top

constexpr int N = 10;
来源：http://rnp.aibaodan.cn

[S58] C++：命名空间
来源：http://ugp.hnxiangtu.top

namespace ns { int f() { return 1; } }
来源：http://xzp.jqgfzy.top

[S59] C++：静态断言
来源：http://kds.yvedp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qgp.chenjidiqi.icu

[S60] C++：遍历并删除元素
来源：http://ahz.hywenlv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://glw.zhixingplan.top

================================================================================
来源：http://gbh.andypj.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yor.yuanzhike.top

================================================================================
来源：http://jze.sweek.top

[T01] Kotlin：Hello World
来源：http://hcw.ppjwa.cn

println("Hello")
来源：http://mfw.chenjidiqi.icu

[T02] Kotlin：变量
来源：http://duc.dianchejie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hej.yueranfly.top


<!-- 参考信息 -->