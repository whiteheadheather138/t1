代发 wailian999

set -euo pipefail
来源：http://izp.c1oappe.top

[R02] 变量赋值与使用
来源：http://yys.wangshuangyany.cn

name="Tom"; echo "$name"
来源：http://yhs.zdqjudy.top

[R03] 只读变量
来源：http://fyx.fengsongda.top

readonly PI=3.14
来源：http://ner.pycfn.com

[R04] 位置参数
来源：http://rhf.yanxiufei.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tlp.bbcook.cn

[R05] 参数默认值
来源：http://cmb.yj202588.top

name="${1:-default}"
来源：http://cit.gzhubu.top

[R06] 判断命令是否存在
来源：http://gtc.hesvh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://aus.316326.xyz

[R07] if 判断文件
来源：http://lpd.feifeiyinyue.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cwl.chenzaomai.com

[R08] 数值比较
来源：http://mea.zhaomingkeji.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://jnu.haohaochexian.top

[R09] 字符串比较
来源：http://kfw.jinyuanbaomall.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pxq.cheryme.top

[R10] 正则匹配
来源：http://sln.svipenyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bci.zhengqikj.top

[R11] case 多分支
来源：http://biv.uphjek.com

case "$1" in
来源：http://zyi.pycfn.com

start) echo "启动" ;;
来源：http://knr.ivvv.top

stop)  echo "停止" ;;
来源：http://arq.zhongyouzk.top

*)     echo "未知命令" ;;
来源：http://sex.ppjwa.cn

esac
来源：http://ngb.wangdashe.top

[R12] for 遍历文件
来源：http://nat.jyoumei.cn

for f in *.txt; do echo "$f"; done
来源：http://kjr.gaohongyu789.top

[R13] for 计数循环
来源：http://yvf.yuxming.cn

for i in {1..10}; do echo "$i"; done
来源：http://mft.gogol.net.cn

[R14] C 风格 for
来源：http://mej.zycfv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hmm.sufxvd.cn

[R15] while 逐行读文件
来源：http://swz.yj202588.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xlu.aibaodan.cn

[R16] until 等待条件
来源：http://oib.wangshuangyany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jqq.sxryk.cn

[R17] 数组定义与取值
来源：http://lzr.dianchejie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bur.andypj.xyz

[R18] 遍历数组
来源：http://pdr.jinyuanbaomall.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nkd.xuanzx.com

[R19] 数组长度
来源：http://fao.iojbl.cn

echo "${#arr[@]}"
来源：http://zfl.feifeiyinyue.top

[R20] 关联数组（字典）
来源：http://mtr.nanxinkj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oav.zhoulong.xyz

[R21] 字符串长度
来源：http://cpg.yvedp.cn

echo "${#s}"
来源：http://zrt.guowangkeji.top

[R22] 截取子串
来源：http://ahf.guannengcc.top

echo "${s:0:5}"
来源：http://bfn.zdqjudy.top

[R23] 字符串替换
来源：http://opj.shzxlz.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qfo.svipenyu.cn

[R24] 大小写转换
来源：http://mhq.sxryk.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mgi.fehbvm.com

[R25] 去后缀 / 去前缀
来源：http://crc.fengsongda.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hxl.jyoumei.cn

[R26] 命令替换
来源：http://qes.0kj1m.cn

now=$(date +%F); echo "$now"
来源：http://rwq.fktsv.cn

[R27] 算术展开
来源：http://lmm.mhx1999.top

echo $((1 + 2 * 3))
来源：http://fwc.daxiang520.top

[R28] 浮点运算
来源：http://myr.zhijiandao.cn

echo "scale=2; 10/3" | bc
来源：http://bgm.ydzc1.top

[R29] 定义函数
来源：http://mjs.epnwcf.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sak.jinyuanbaomall.cn

[R30] 函数返回状态码
来源：http://sum.yfazqb.com

f() { return 0; }; f || echo "失败了"
来源：http://kok.wangshuangyany.cn

[R31] 局部变量
来源：http://rbk.hnqzz.top

f() { local x=1; echo "$x"; }
来源：http://yrv.guannengcc.top

[R32] 参数个数校验
来源：http://rfk.pengpengdd.cyou

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ase.ppjwa.cn

[R33] 捕获错误并提示行号
来源：http://oaa.sjlbkw.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://exr.havefunace.top

[R34] 退出时清理
来源：http://sqz.ehwqpu.com

trap 'rm -f "$tmp"' EXIT
来源：http://qys.zycfv.cn

[R35] 后台执行并等待
来源：http://onv.sweek.top

sleep 5 & pid=$!; wait "$pid"
来源：http://qea.nwbrower.top

[R36] 并发执行多个任务
来源：http://iaz.xziqi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ucr.cdnleiting.top

[R37] 把输出赋给变量
来源：http://jda.yj202588.top

files=$(ls -1)
来源：http://qtg.jinqigufen.top

[R38] 管道串联
来源：http://twb.ydzc1.top

cat a.txt | grep -i error | wc -l
来源：http://rpo.fanxiaobao.xyz

[R39] 重定向标准输出与错误
来源：http://cow.nwbrower.top

cmd > out.log 2>&1
来源：http://qia.shzxlz.cn

[R40] 追加写日志
来源：http://iub.cashguo.top

echo "log" >> out.log
来源：http://uku.jyoumei.cn

[R41] 丢弃输出
来源：http://jpr.jinyuanbaomall.cn

cmd >/dev/null 2>&1
来源：http://jav.cheryme.top

[R42] 输入重定向
来源：http://zjr.zhixingplan.top

wc -l < a.txt
来源：http://rtg.xuanzx.com

[R43] 按名字查找文件
来源：http://dli.tanke756.top

find . -name "*.log" -type f
来源：http://vqd.9152youxi.cn

[R44] 按修改时间查找
来源：http://llg.yueranfly.top

find . -mtime -7 -type f
来源：http://ojw.yuanzhike.top

[R45] 批量删除
来源：http://ony.jinyuanbaomall.cn

find . -name "*.tmp" -delete
来源：http://hqx.quarkkingdee.top

[R46] 递归替换文件内容
来源：http://rok.gogol.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dnm.aizwys.cn

[R47] sed 单行替换
来源：http://vkh.yonumen.top

sed -i 's/foo/bar/g' a.txt
来源：http://xjw.wangshuangyany.cn

[R48] awk 取指定列
来源：http://qem.nanxinkj.top

awk '{print $1, $3}' a.txt
来源：http://gxw.birdmap.top

[R49] awk 带条件
来源：http://rpj.vqdsnc.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wse.wangshuangyany.cn

[R50] awk 求和
来源：http://wfw.sjlbkw.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qgr.ivvv.top

[R51] 排序去重取前几
来源：http://xaf.xingfuxueyuan.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://uyy.shanyushiyangkeji.top

[R52] 统计行数
来源：http://ssu.ehwqpu.com

wc -l a.txt
来源：http://ncm.svipenyu.cn

[R53] 查看文件头与实时尾
来源：http://dwj.xinyue.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dbc.sxryk.cn

[R54] 比较两个文件
来源：http://rdd.aizwys.cn

diff a.txt b.txt
来源：http://rsv.tian-w.cn

[R55] 压缩与解压
来源：http://egs.0kj1m.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vxh.zhixingplan.top

[R56] 远程拷贝
来源：http://yeu.shanyushiyangtech.top

scp file user@host:/path/
来源：http://lmn.gotoacloud.top

[R57] 远程执行命令
来源：http://rvz.epnwcf.com

ssh user@host 'uptime'
来源：http://qzc.hesvh.cn

[R58] 下载文件
来源：http://jrc.pycfn.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zmm.mhx1999.top

[R59] 发 POST JSON
来源：http://rgm.shzxlz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cvc.andypj.xyz

[R60] 只看 HTTP 状态码
来源：http://mlf.ctjpmb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hpl.ehwqpu.com

[R61] 磁盘占用
来源：http://ljm.iojbl.cn

df -h;  du -sh *
来源：http://evn.jinghuilouyu.cn

[R62] 找最占空间的文件
来源：http://atv.zdbjq.cn

du -ah . | sort -rh | head -10
来源：http://pjm.xylfe.cn

[R63] 内存与进程
来源：http://yct.zhoulong.xyz

free -h;  ps aux | grep nginx
来源：http://klp.fanxiaobao.xyz

[R64] 结束进程
来源：http://msl.jinyuanbaomall.cn

kill -9 $(pgrep -f app.py)
来源：http://rvn.bjfxy.top

[R65] 查看端口占用
来源：http://npa.sufxvd.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hah.tarul.cn

[R66] 定时任务
来源：http://zcs.fanxiaobao.xyz

crontab -e;  crontab -l
来源：http://jkx.yfazqb.com

[R67] 生成随机十六进制串
来源：http://mrd.xziqi.cn

openssl rand -hex 16
来源：http://ihw.havefunace.top

[R68] 计算文件校验值
来源：http://hax.ctjpmb.com

sha256sum a.txt;  md5sum a.txt
来源：http://ofq.feifeiyinyue.top

[R69] 生成随机密码
来源：http://bex.fktsv.cn

head -c 16 /dev/urandom | base64
来源：http://olx.sxryk.cn

[R70] 时间戳与互转
来源：http://wqr.zhengqikj.top

date +%s;  date -d @1700000000
来源：http://bvp.gzhubu.top

[R71] 日期格式化
来源：http://lta.yuxming.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://afs.shanyushiyangkeji.top

[R72] 等待端口就绪
来源：http://hki.cdnleiting.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vpf.havefunace.top

[R73] 分割大日志
来源：http://dov.yj202588.top

split -l 1000 big.log part_
来源：http://ylk.ybcxt.top

[R74] 批量重命名
来源：http://srd.quarkkingdee.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lms.yuxming.cn

[R75] 导出环境变量
来源：http://ygw.dianchejie.cn

export PATH="$HOME/bin:$PATH"
来源：http://ufw.52xcode.cn

[R76] 使用临时文件
来源：http://ixa.wangdashe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lux.ydzc1.top

[R77] 读取用户输入
来源：http://sus.gogol.net.cn

read -rp "请输入: " ans
来源：http://bqz.jinqigufen.top

[R78] 交互式菜单
来源：http://mfu.svipenyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bbl.svipenyu.cn

[R79] 解析命令行选项
来源：http://fox.guowangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oiv.hysaishi.cn

[R80] 查看脚本执行耗时
来源：http://kbn.feifeiyinyue.top

time ./run.sh
来源：http://ruy.cucudq.cn

================================================================================
来源：http://few.guannengcc.top

S. C / C++ 专题
来源：http://urp.hnqzz.top

================================================================================
来源：http://zph.andypj.xyz

[S01] C：Hello World
来源：http://lfr.fktsv.cn

#include <stdio.h>
来源：http://yzm.xuanzx.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://hbq.daria6918.cn

[S02] C：变量与格式化输出
来源：http://cbf.zdbjq.cn

int a = 10; printf("%d\n", a);
来源：http://bcv.yvedp.cn

[S03] C：读入整数
来源：http://ixd.316326.xyz

int x; scanf("%d", &x);
来源：http://mjy.shangyingyoupin.top

[S04] C：字符串复制
来源：http://hhy.smart0.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://pyb.0kj1m.cn

[S05] C：字符串长度
来源：http://rgi.aizwys.cn

strlen(s)
来源：http://lgm.fehbvm.com

[S06] C：字符串比较
来源：http://uqy.hesvh.cn

strcmp(a, b) == 0
来源：http://lus.andypj.xyz

[S07] C：数组遍历求和
来源：http://ivc.ydjk.org.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://aci.yonumen.top

[S08] C：动态内存分配与释放
来源：http://yvd.gzhubu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://avw.cqqwz.cn

[S09] C：结构体定义与初始化
来源：http://aes.cdnleiting.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lpb.andypj.xyz

[S10] C：指针与解引用
来源：http://isk.hongshengwenyu.top

int *p = &a;  *p = 5;
来源：http://cbi.tanke756.top

[S11] C：逐行读文件
来源：http://jyv.yj20258.top

FILE *f = fopen("a.txt", "r");
来源：http://rlw.jinghuilouyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qfa.aizwys.cn

fclose(f);
来源：http://vco.aibaodan.cn

[S12] C：写文件
来源：http://dot.pycfn.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gxd.c1oappe.top

[S13] C：宏定义
来源：http://ktq.0kj1m.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ery.gogol.net.cn

[S14] C：枚举
来源：http://jhm.meibo888.top

enum Color { RED, GREEN, BLUE };
来源：http://mdk.ydjk.org.cn

[S15] C：类型转换
来源：http://tsi.zhiwuduotai.top

(double) a / b
来源：http://lmr.yj20258.top

[S16] C：位操作置位
来源：http://lak.jinqigufen.top

x |= (1 << 3);
来源：http://wmj.nwbrower.top

[S17] C：安全拼接字符串
来源：http://pwr.hesvh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hyt.kuanghao11.cn

[S18] C：命令行参数
来源：http://gog.haohaochexian.top

int main(int argc, char **argv)
来源：http://gai.fanxiaobao.xyz

[S19] C：快速排序
来源：http://nyb.shzxlz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dic.jqgufenzy.top

[S20] C：二分查找
来源：http://rgi.jinghuilouyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ifd.epnwcf.com

[S21] C：字符类别判断
来源：http://kkm.jiagoushi.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jat.redwolf501.top

[S22] C：字符串转数字
来源：http://wba.jyoumei.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dlu.316326.xyz

[S23] C：随机数
来源：http://bax.cdnleiting.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dao.tarul.cn

[S24] C：获取本地时间
来源：http://vts.yonumen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qnj.c1oappe.top

[S25] C：内存拷贝
来源：http://dhb.hnqzz.top

memcpy(dst, src, n);
来源：http://teq.cashguo.top

[S26] C：内存清零
来源：http://azc.dashuyun.cn

memset(a, 0, sizeof a);
来源：http://kzg.yvedp.cn

[S27] C：定义常量
来源：http://edm.aibaodan.cn

const double PI = 3.14159;
来源：http://tdu.yuanzhike.top

[S28] C：静态变量
来源：http://ffg.xziqi.cn

static int counter = 0;
来源：http://yva.yfazqb.com

[S29] C：变参函数
来源：http://zwf.sufxvd.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jlv.yanxiufei.cn

[S30] C：头文件保护
来源：http://rks.vqdsnc.cn

#ifndef X_H
来源：http://nvi.xuetiantiany.cn

#define X_H
来源：http://yaq.pycfn.com

#endif
来源：http://fbh.yonumen.top

[S31] C++：Hello World
来源：http://zci.sufxvd.cn

#include <iostream>
来源：http://fak.sxryk.cn

int main() { std::cout << "Hello\n"; }
来源：http://sbx.vehdjk.com

[S32] C++：字符串
来源：http://sqg.shanyushiyangtech.top

std::string s = "hi";  s += "!";
来源：http://vnz.zdqjudy.top

[S33] C++：vector 增删
来源：http://tef.snrcjt.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iky.zycfv.cn

[S34] C++：遍历 vector
来源：http://qet.daxiang520.top

for (auto &x : v) { std::cout << x; }
来源：http://hyh.0kj1m.cn

[S35] C++：map
来源：http://mni.sysykeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lwe.gogol.net.cn

[S36] C++：unordered_map
来源：http://mos.vehdjk.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://alh.cheryme.top

[S37] C++：set
来源：http://nyv.epnwcf.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jyy.vehdjk.com

[S38] C++：排序
来源：http://oaa.shanyushiyangkeji.top

std::sort(v.begin(), v.end());
来源：http://lpi.zhixingplan.top

[S39] C++：自定义比较器排序
来源：http://wux.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lzd.cucudq.cn

[S40] C++：查找元素
来源：http://bco.sufxvd.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ywj.cdnleiting.top

[S41] C++：类与构造函数
来源：http://olc.meibo888.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zbx.chenzaomai.com

[S42] C++：继承与虚函数
来源：http://rgp.guannengcc.top

class B : public Base { public: void f() override {} };
来源：http://nbg.yj202588.top

[S43] C++：智能指针
来源：http://dgu.birdmap.top

auto p = std::make_unique<int>(5);
来源：http://qbm.hysaishi.cn

[S44] C++：引用传参
来源：http://ifw.316326.xyz

void inc(int &x) { ++x; }
来源：http://jzt.yangfankeji.com

[S45] C++：lambda
来源：http://bxo.hcnkem.com

auto add = [](int a, int b) { return a + b; };
来源：http://fbg.daria6918.cn

[S46] C++：函数模板
来源：http://xcm.yangfankeji.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oxe.haohaochexian.top

[S47] C++：结构化绑定遍历
来源：http://ztp.ydzc1.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nzt.chenlongwang.top

[S48] C++：逐行读文件
来源：http://jzk.ybcxt.top

std::ifstream in("a.txt");  std::string line;
来源：http://fjc.vqdsnc.cn

while (std::getline(in, line)) { }
来源：http://uhn.yuanzhike.top

[S49] C++：写文件
来源：http://iar.tianlin.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://agk.jinyuanbaomall.cn

[S50] C++：格式化数字
来源：http://lwp.zhongyouzk.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jih.yangfankeji.com

[S51] C++：显式类型转换
来源：http://bjq.yangfankeji.com

static_cast<double>(a) / b
来源：http://yop.gotoacloud.top

[S52] C++：const 与 noexcept
来源：http://egm.bbcook.cn

int size() const noexcept { return n_; }
来源：http://xfp.birdmap.top

[S53] C++：移动语义
来源：http://soh.fehbvm.com

std::vector<int> w = std::move(v);
来源：http://hgr.xylfe.cn

[S54] C++：异常处理
来源：http://nod.cqqwz.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ipi.yonumen.top

[S55] C++：结构化绑定
来源：http://lux.zdqjudy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://fel.jyoumei.cn

[S56] C++：optional
来源：http://zxb.52xcode.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mbr.daria6918.cn

[S57] C++：编译期常量
来源：http://bhu.zhoulong.xyz

constexpr int N = 10;
来源：http://bxm.sysykeji.top

[S58] C++：命名空间
来源：http://zsv.vqdsnc.cn

namespace ns { int f() { return 1; } }
来源：http://bvh.ctjpmb.com

[S59] C++：静态断言
来源：http://bbw.nanxuanxn.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yzb.vqdsnc.cn

[S60] C++：遍历并删除元素
来源：http://gqv.jinyuanbaomall.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://aay.sxryk.cn

================================================================================
来源：http://cdh.shuidangran.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://arl.dianchejie.cn

================================================================================
来源：http://mhu.hesvh.cn

[T01] Kotlin：Hello World
来源：http://qwm.ybcxt.top

println("Hello")
来源：http://cte.tarul.cn

[T02] Kotlin：变量
来源：http://qzt.cashguo.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lmu.bbcook.cn


<!-- 参考信息 -->