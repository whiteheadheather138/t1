代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gix.xuetiantiany.cn

[Q90] 生成序号列
来源：http://iiu.zhaomingkeji.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ays.yueranfly.top

================================================================================
来源：http://nij.jinyuanbaomall.cn

R. Bash 专题
来源：http://ysg.hesvh.cn

================================================================================
来源：http://dpd.dianchejie.cn

[R01] shebang 与严格模式
来源：http://whh.cqqwz.cn

#!/usr/bin/env bash
来源：http://hed.chenlongwang.top

set -euo pipefail
来源：http://rrz.xziqi.cn

[R02] 变量赋值与使用
来源：http://ejr.hongshengwenyu.top

name="Tom"; echo "$name"
来源：http://nrd.kuanghao11.cn

[R03] 只读变量
来源：http://cty.hnqzz.top

readonly PI=3.14
来源：http://oxs.svipenyu.cn

[R04] 位置参数
来源：http://cea.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sib.sjlbkw.cn

[R05] 参数默认值
来源：http://rsf.zhiwuduotai.top

name="${1:-default}"
来源：http://psa.sxryk.cn

[R06] 判断命令是否存在
来源：http://mda.hammf.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hle.daxiang520.top

[R07] if 判断文件
来源：http://xan.cqqwz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nas.yongpay.top

[R08] 数值比较
来源：http://cpg.ywan-chungtsiang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://osz.jinghuilouyu.cn

[R09] 字符串比较
来源：http://jzn.gzhubu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vte.ehwqpu.com

[R10] 正则匹配
来源：http://rto.chenzaomai.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kno.gotoacloud.top

[R11] case 多分支
来源：http://htk.aibaodan.cn

case "$1" in
来源：http://efy.yanxiufei.cn

start) echo "启动" ;;
来源：http://fdz.guannengcc.top

stop)  echo "停止" ;;
来源：http://hcl.smart0.xyz

*)     echo "未知命令" ;;
来源：http://prf.feifeiyinyue.top

esac
来源：http://dxk.yfazqb.com

[R12] for 遍历文件
来源：http://ipl.andypj.xyz

for f in *.txt; do echo "$f"; done
来源：http://gro.hongshengwenyu.top

[R13] for 计数循环
来源：http://kxg.shzxlz.cn

for i in {1..10}; do echo "$i"; done
来源：http://dzr.yuanzhike.top

[R14] C 风格 for
来源：http://mqf.yueranfly.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fgn.jqgufenzy.top

[R15] while 逐行读文件
来源：http://uzp.shangyingyoupin.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ojc.havefunace.top

[R16] until 等待条件
来源：http://hlc.vehdjk.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jih.zdqjudy.top

[R17] 数组定义与取值
来源：http://qai.sysykeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://xxx.quarkkingdee.top

[R18] 遍历数组
来源：http://xsl.wangdashe.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tms.ywan-chungtsiang.top

[R19] 数组长度
来源：http://fst.0kj1m.cn

echo "${#arr[@]}"
来源：http://ksx.epnwcf.com

[R20] 关联数组（字典）
来源：http://wlh.jlsjyb.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://msz.chenjidiqi.icu

[R21] 字符串长度
来源：http://ibm.yongpay.top

echo "${#s}"
来源：http://qcm.hfpthk.cn

[R22] 截取子串
来源：http://zrs.zhoulong.xyz

echo "${s:0:5}"
来源：http://nlh.wangdashe.top

[R23] 字符串替换
来源：http://fzn.havefunace.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tdq.shangyingyoupin.top

[R24] 大小写转换
来源：http://bht.tianlin.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://lev.snrcjt.cn

[R25] 去后缀 / 去前缀
来源：http://dfj.jianghu66.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vor.uphjek.com

[R26] 命令替换
来源：http://uzc.cheryme.top

now=$(date +%F); echo "$now"
来源：http://fxf.nwbrower.top

[R27] 算术展开
来源：http://xos.andypj.xyz

echo $((1 + 2 * 3))
来源：http://shi.hfpthk.cn

[R28] 浮点运算
来源：http://rnb.yj202588.top

echo "scale=2; 10/3" | bc
来源：http://xog.shanyushiyangkeji.top

[R29] 定义函数
来源：http://wfe.zhongyouzk.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gqw.yongpay.top

[R30] 函数返回状态码
来源：http://ozz.jyoumei.cn

f() { return 0; }; f || echo "失败了"
来源：http://xfx.sjlbkw.cn

[R31] 局部变量
来源：http://gqc.fzhhl.top

f() { local x=1; echo "$x"; }
来源：http://iue.birdmap.top

[R32] 参数个数校验
来源：http://igw.jqgufenzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vge.52xcode.cn

[R33] 捕获错误并提示行号
来源：http://zyw.c1oappe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nda.xuetiantiany.cn

[R34] 退出时清理
来源：http://xgo.tarul.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rwv.nanxinkj.top

[R35] 后台执行并等待
来源：http://cnj.0kj1m.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pfm.jinqigufen.top

[R36] 并发执行多个任务
来源：http://zoz.dashuyun.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hbb.sjlbkw.cn

[R37] 把输出赋给变量
来源：http://bls.snrcjt.cn

files=$(ls -1)
来源：http://gyb.tian-w.cn

[R38] 管道串联
来源：http://bci.hesvh.cn

cat a.txt | grep -i error | wc -l
来源：http://scl.daxiang520.top

[R39] 重定向标准输出与错误
来源：http://jhw.vehdjk.com

cmd > out.log 2>&1
来源：http://pkn.chenlongwang.top

[R40] 追加写日志
来源：http://aoe.dianchejie.cn

echo "log" >> out.log
来源：http://wed.xingfuxueyuan.xyz

[R41] 丢弃输出
来源：http://pdm.fzhhl.top

cmd >/dev/null 2>&1
来源：http://rec.jianghu66.top

[R42] 输入重定向
来源：http://smx.yj20258.top

wc -l < a.txt
来源：http://ofc.shuidangran.top

[R43] 按名字查找文件
来源：http://dqg.xinyue.icu

find . -name "*.log" -type f
来源：http://fpg.jinqigfzy.top

[R44] 按修改时间查找
来源：http://fyb.shangyingyoupin.top

find . -mtime -7 -type f
来源：http://rui.zdbjq.cn

[R45] 批量删除
来源：http://tsf.guowangkeji.top

find . -name "*.tmp" -delete
来源：http://uml.svipenyu.cn

[R46] 递归替换文件内容
来源：http://xeb.jyoumei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fhb.gogol.net.cn

[R47] sed 单行替换
来源：http://zxs.ppjwa.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zpk.tian-w.cn

[R48] awk 取指定列
来源：http://vsh.fktsv.cn

awk '{print $1, $3}' a.txt
来源：http://tra.nanxinkj.top

[R49] awk 带条件
来源：http://cej.sweek.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://egk.tarul.cn

[R50] awk 求和
来源：http://ecg.ywan-chungtsiang.top

awk '{s += $2} END {print s}' a.txt
来源：http://ljf.guannengcc.top

[R51] 排序去重取前几
来源：http://mph.tanke756.top

sort a.txt | uniq -c | sort -rn | head
来源：http://xsi.aizwys.cn

[R52] 统计行数
来源：http://zil.sysykeji.top

wc -l a.txt
来源：http://ygq.vqdsnc.cn

[R53] 查看文件头与实时尾
来源：http://nec.zycfv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://boe.andypj.xyz

[R54] 比较两个文件
来源：http://epm.zhaomingkeji.xyz

diff a.txt b.txt
来源：http://qlk.xinyue.icu

[R55] 压缩与解压
来源：http://zsk.hywenlv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iye.tarul.cn

[R56] 远程拷贝
来源：http://pxy.sxryk.cn

scp file user@host:/path/
来源：http://qdy.ehwqpu.com

[R57] 远程执行命令
来源：http://kyo.yueranfly.top

ssh user@host 'uptime'
来源：http://mvv.tian-w.cn

[R58] 下载文件
来源：http://gqq.ydzc1.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eku.jinqigufen.top

[R59] 发 POST JSON
来源：http://kzw.yuxming.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jqj.gogol.net.cn

[R60] 只看 HTTP 状态码
来源：http://ghd.yj202588.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xpw.quarkkingdee.top

[R61] 磁盘占用
来源：http://iwl.gotoacloud.top

df -h;  du -sh *
来源：http://ldr.316326.xyz

[R62] 找最占空间的文件
来源：http://sdi.shzxlz.cn

du -ah . | sort -rh | head -10
来源：http://rnw.chenzaomai.com

[R63] 内存与进程
来源：http://pkt.0kj1m.cn

free -h;  ps aux | grep nginx
来源：http://wws.hnqzz.top

[R64] 结束进程
来源：http://wdd.zhiwuduotai.top

kill -9 $(pgrep -f app.py)
来源：http://jco.fzhhl.top

[R65] 查看端口占用
来源：http://fzs.tanke756.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://iet.hcnkem.com

[R66] 定时任务
来源：http://mah.gzhubu.top

crontab -e;  crontab -l
来源：http://nmu.ydzc1.top

[R67] 生成随机十六进制串
来源：http://gjm.shuidangran.top

openssl rand -hex 16
来源：http://ula.ydzc1.top

[R68] 计算文件校验值
来源：http://jnw.zdbjq.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jac.dashuyun.cn

[R69] 生成随机密码
来源：http://gkr.tanke756.top

head -c 16 /dev/urandom | base64
来源：http://mfg.hnqzz.top

[R70] 时间戳与互转
来源：http://kec.iojbl.cn

date +%s;  date -d @1700000000
来源：http://eki.fehbvm.com

[R71] 日期格式化
来源：http://orj.dashuyun.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uxe.wangdashe.top

[R72] 等待端口就绪
来源：http://cez.guannengcc.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nkh.hnxiangtu.top

[R73] 分割大日志
来源：http://ect.zhaomingkeji.xyz

split -l 1000 big.log part_
来源：http://wbj.shangyingyoupin.top

[R74] 批量重命名
来源：http://wca.0kj1m.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://igo.pycfn.com

[R75] 导出环境变量
来源：http://uyg.c1oappe.top

export PATH="$HOME/bin:$PATH"
来源：http://tsq.yuxming.cn

[R76] 使用临时文件
来源：http://bga.ctjpmb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kst.hcnkem.com

[R77] 读取用户输入
来源：http://tnp.aibaodan.cn

read -rp "请输入: " ans
来源：http://izv.jinqigufen.top

[R78] 交互式菜单
来源：http://mbc.ivvv.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ugt.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://dig.yj20258888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ejq.hammf.cn

[R80] 查看脚本执行耗时
来源：http://tiw.ywan-chungtsiang.top

time ./run.sh
来源：http://lkx.yj202588.top

================================================================================
来源：http://byi.zdqjudy.top

S. C / C++ 专题
来源：http://nin.yangfankeji.com

================================================================================
来源：http://kyd.xziqi.cn

[S01] C：Hello World
来源：http://hic.tianlin.xyz

#include <stdio.h>
来源：http://gyw.yongpay.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://hth.jqgfzy.top

[S02] C：变量与格式化输出
来源：http://vda.epnwcf.com

int a = 10; printf("%d\n", a);
来源：http://vdt.bjfxy.top

[S03] C：读入整数
来源：http://acn.zhiwuduotai.top

int x; scanf("%d", &x);
来源：http://vic.nanxinkj.top

[S04] C：字符串复制
来源：http://krc.cqqwz.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rjz.smart0.xyz

[S05] C：字符串长度
来源：http://lbd.yj20258888.top

strlen(s)
来源：http://syq.hywenlv.cn

[S06] C：字符串比较
来源：http://wpi.fktsv.cn

strcmp(a, b) == 0
来源：http://bse.xziqi.cn

[S07] C：数组遍历求和
来源：http://tfn.jqgufenzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gbw.fengsongda.top

[S08] C：动态内存分配与释放
来源：http://zdj.tanke756.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://isc.ybcxt.top

[S09] C：结构体定义与初始化
来源：http://vvp.zhengqikj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ago.hammf.cn

[S10] C：指针与解引用
来源：http://nyh.gzhubu.top

int *p = &a;  *p = 5;
来源：http://knp.jianghu66.top

[S11] C：逐行读文件
来源：http://gyy.sweek.top

FILE *f = fopen("a.txt", "r");
来源：http://gdq.fehbvm.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://jjj.jqgufenzy.top

fclose(f);
来源：http://yzg.aizwys.cn

[S12] C：写文件
来源：http://bwg.tanke756.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wbb.dashuyun.cn

[S13] C：宏定义
来源：http://eci.jlsjyb.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ind.xingfuxueyuan.xyz

[S14] C：枚举
来源：http://zed.yuanzhike.top

enum Color { RED, GREEN, BLUE };
来源：http://gge.jinghuilouyu.cn

[S15] C：类型转换
来源：http://ofe.zhixingplan.top

(double) a / b
来源：http://xiq.0kj1m.cn

[S16] C：位操作置位
来源：http://xuc.cashguo.top

x |= (1 << 3);
来源：http://pde.ppjwa.cn

[S17] C：安全拼接字符串
来源：http://vxx.ivvv.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baw.yanxiufei.cn

[S18] C：命令行参数
来源：http://gvj.zhaomingkeji.xyz

int main(int argc, char **argv)
来源：http://jbk.mhx1999.top

[S19] C：快速排序
来源：http://drx.feifeiyinyue.top

qsort(a, n, sizeof(int), cmp);
来源：http://zuj.xingfuxueyuan.xyz

[S20] C：二分查找
来源：http://ojt.aizwys.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wkl.ehwqpu.com

[S21] C：字符类别判断
来源：http://zxz.guannengcc.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zvt.chenlongwang.top

[S22] C：字符串转数字
来源：http://wjb.jinyuanbaomall.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lrq.zhiwuduotai.top

[S23] C：随机数
来源：http://wqr.yueranfly.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dig.zhaomingkeji.xyz

[S24] C：获取本地时间
来源：http://loq.tian-w.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ufl.hammf.cn

[S25] C：内存拷贝
来源：http://pdu.ctjpmb.com

memcpy(dst, src, n);
来源：http://rha.cheryme.top

[S26] C：内存清零
来源：http://wws.quarkkingdee.top

memset(a, 0, sizeof a);
来源：http://fle.tanke756.top

[S27] C：定义常量
来源：http://tee.sufxvd.cn

const double PI = 3.14159;
来源：http://war.bbcook.cn

[S28] C：静态变量
来源：http://tmn.ctjpmb.com

static int counter = 0;
来源：http://wzn.hysaishi.cn

[S29] C：变参函数
来源：http://dhb.yvedp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://awy.0kj1m.cn

[S30] C：头文件保护
来源：http://hdl.jianghu66.top

#ifndef X_H
来源：http://ofn.yj20258888.top

#define X_H
来源：http://yno.0kj1m.cn

#endif
来源：http://ohb.pengpengdd.cyou

[S31] C++：Hello World
来源：http://dyy.jyoumei.cn

#include <iostream>
来源：http://yid.yanxiufei.cn

int main() { std::cout << "Hello\n"; }
来源：http://hux.jlsjyb.cn

[S32] C++：字符串
来源：http://zzb.tarul.cn

std::string s = "hi";  s += "!";
来源：http://pdz.xuanzx.com

[S33] C++：vector 增删
来源：http://cig.ivvv.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lhr.9152youxi.cn

[S34] C++：遍历 vector
来源：http://csv.vqdsnc.cn

for (auto &x : v) { std::cout << x; }
来源：http://acf.jinqigfzy.top

[S35] C++：map
来源：http://awj.chenjidiqi.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hlm.ivvv.top

[S36] C++：unordered_map
来源：http://lct.fengsongda.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wcn.daria6918.cn

[S37] C++：set
来源：http://zsg.xingfuxueyuan.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vel.daria6918.cn

[S38] C++：排序
来源：http://riv.yfazqb.com

std::sort(v.begin(), v.end());
来源：http://axj.sysykeji.top

[S39] C++：自定义比较器排序
来源：http://xkv.jiagoushi.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://abw.sjlbkw.cn

[S40] C++：查找元素
来源：http://vyo.jqgfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jdp.snrcjt.cn

[S41] C++：类与构造函数
来源：http://diw.ydjk.org.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bpn.yj202588.top

[S42] C++：继承与虚函数
来源：http://sxh.fzhhl.top

class B : public Base { public: void f() override {} };
来源：http://bty.andypj.xyz

[S43] C++：智能指针
来源：http://npc.quarkkingdee.top

auto p = std::make_unique<int>(5);
来源：http://zar.birdmap.top

[S44] C++：引用传参
来源：http://sbi.havefunace.top

void inc(int &x) { ++x; }
来源：http://wni.ehwqpu.com

[S45] C++：lambda
来源：http://gbl.zhongyouzk.top

auto add = [](int a, int b) { return a + b; };
来源：http://swe.shuidangran.top

[S46] C++：函数模板
来源：http://cut.yfazqb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lvk.dianchejie.cn

[S47] C++：结构化绑定遍历
来源：http://ggj.wangdashe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jaf.yvedp.cn

[S48] C++：逐行读文件
来源：http://bto.zdqjudy.top

std::ifstream in("a.txt");  std::string line;
来源：http://emg.nanxuanxn.top

while (std::getline(in, line)) { }
来源：http://dtw.bbcook.cn

[S49] C++：写文件
来源：http://juo.cdnleiting.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kug.sxryk.cn

[S50] C++：格式化数字
来源：http://hvq.yuxming.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fzm.316326.xyz

[S51] C++：显式类型转换
来源：http://otu.yonumen.top

static_cast<double>(a) / b
来源：http://vtn.wangshuangyany.cn

[S52] C++：const 与 noexcept
来源：http://ouq.svipenyu.cn

int size() const noexcept { return n_; }
来源：http://hog.hesvh.cn

[S53] C++：移动语义
来源：http://rah.zycfv.cn

std::vector<int> w = std::move(v);
来源：http://cnx.ctjpmb.com

[S54] C++：异常处理
来源：http://xpy.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jku.nanxuanxn.top

[S55] C++：结构化绑定
来源：http://ctw.jinyuanbaomall.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ihr.svipenyu.cn

[S56] C++：optional
来源：http://tiq.zhoulong.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cxp.cashguo.top

[S57] C++：编译期常量
来源：http://vno.havefunace.top

constexpr int N = 10;
来源：http://yno.ywan-chungtsiang.top

[S58] C++：命名空间
来源：http://vuw.cashguo.top

namespace ns { int f() { return 1; } }
来源：http://mqt.sxryk.cn

[S59] C++：静态断言
来源：http://lqv.jqgfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zgv.jianghu66.top

[S60] C++：遍历并删除元素
来源：http://bdd.tian-w.cn


<!-- 参考信息 -->