代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rer.zhixingplan.top

[Q90] 生成序号列
来源：http://ppf.pycfn.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xbm.tian-w.cn

================================================================================
来源：http://zmz.xuetiantiany.cn

R. Bash 专题
来源：http://qsg.pycfn.com

================================================================================
来源：http://fqm.vqdsnc.cn

[R01] shebang 与严格模式
来源：http://sku.cashguo.top

#!/usr/bin/env bash
来源：http://wej.9152youxi.cn

set -euo pipefail
来源：http://rme.meibo888.top

[R02] 变量赋值与使用
来源：http://iki.sxryk.cn

name="Tom"; echo "$name"
来源：http://hvl.tianlin.xyz

[R03] 只读变量
来源：http://jre.snrcjt.cn

readonly PI=3.14
来源：http://bvm.sweek.top

[R04] 位置参数
来源：http://nun.hesvh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://inp.dianchejie.cn

[R05] 参数默认值
来源：http://bwc.gogol.net.cn

name="${1:-default}"
来源：http://jln.yj202588.top

[R06] 判断命令是否存在
来源：http://pfo.wangshuangyany.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ttj.yonumen.top

[R07] if 判断文件
来源：http://fcm.sweek.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://epn.nanxinkj.top

[R08] 数值比较
来源：http://xtg.shangyingyoupin.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ozm.fzhhl.top

[R09] 字符串比较
来源：http://wxc.mhx1999.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://alr.jinqigufen.top

[R10] 正则匹配
来源：http://lzp.guannengcc.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://thk.hammf.cn

[R11] case 多分支
来源：http://rfr.jinqigfzy.top

case "$1" in
来源：http://suq.9152youxi.cn

start) echo "启动" ;;
来源：http://ycn.52xcode.cn

stop)  echo "停止" ;;
来源：http://tmy.shanyushiyangtech.top

*)     echo "未知命令" ;;
来源：http://nbo.ybcxt.top

esac
来源：http://smi.316326.xyz

[R12] for 遍历文件
来源：http://vnq.0kj1m.cn

for f in *.txt; do echo "$f"; done
来源：http://elj.sxryk.cn

[R13] for 计数循环
来源：http://aqt.yj20258888.top

for i in {1..10}; do echo "$i"; done
来源：http://php.gzhubu.top

[R14] C 风格 for
来源：http://qbb.sjlbkw.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://onh.guowangkeji.top

[R15] while 逐行读文件
来源：http://oet.vqdsnc.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wgq.xylfe.cn

[R16] until 等待条件
来源：http://ktu.hesvh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://utq.fengsongda.top

[R17] 数组定义与取值
来源：http://dek.haohaochexian.top

arr=(a b c); echo "${arr[0]}"
来源：http://wwq.aibaodan.cn

[R18] 遍历数组
来源：http://gdy.chenzaomai.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://smz.yangfankeji.com

[R19] 数组长度
来源：http://ifg.aizwys.cn

echo "${#arr[@]}"
来源：http://ehb.havefunace.top

[R20] 关联数组（字典）
来源：http://gqs.fanxiaobao.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://abr.zycfv.cn

[R21] 字符串长度
来源：http://zuw.yonumen.top

echo "${#s}"
来源：http://iez.0kj1m.cn

[R22] 截取子串
来源：http://sxx.sjlbkw.cn

echo "${s:0:5}"
来源：http://gyb.316326.xyz

[R23] 字符串替换
来源：http://tiq.cashguo.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ajp.tanke756.top

[R24] 大小写转换
来源：http://xkf.ppjwa.cn

echo "${s^^}"; echo "${s,,}"
来源：http://guf.cdnleiting.top

[R25] 去后缀 / 去前缀
来源：http://xnu.ehwqpu.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://lsf.sysykeji.top

[R26] 命令替换
来源：http://gkz.yuxming.cn

now=$(date +%F); echo "$now"
来源：http://baj.tian-w.cn

[R27] 算术展开
来源：http://duj.zdbjq.cn

echo $((1 + 2 * 3))
来源：http://cvr.sysykeji.top

[R28] 浮点运算
来源：http://typ.cdnleiting.top

echo "scale=2; 10/3" | bc
来源：http://ito.zycfv.cn

[R29] 定义函数
来源：http://ccd.zhoulong.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://svp.hammf.cn

[R30] 函数返回状态码
来源：http://xzy.yonumen.top

f() { return 0; }; f || echo "失败了"
来源：http://buu.cdnleiting.top

[R31] 局部变量
来源：http://ikn.chenzaomai.com

f() { local x=1; echo "$x"; }
来源：http://qeb.hesvh.cn

[R32] 参数个数校验
来源：http://aqm.haohaochexian.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ufn.epnwcf.com

[R33] 捕获错误并提示行号
来源：http://jht.316326.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://luj.zdbjq.cn

[R34] 退出时清理
来源：http://dtl.ydjk.org.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dps.xingfuxueyuan.xyz

[R35] 后台执行并等待
来源：http://yyc.cqqwz.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vdo.pycfn.com

[R36] 并发执行多个任务
来源：http://hln.jinqigufen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ojl.sxryk.cn

[R37] 把输出赋给变量
来源：http://vbx.316326.xyz

files=$(ls -1)
来源：http://lep.zycfv.cn

[R38] 管道串联
来源：http://qcc.hnqzz.top

cat a.txt | grep -i error | wc -l
来源：http://izu.redwolf501.top

[R39] 重定向标准输出与错误
来源：http://rvv.fanxiaobao.xyz

cmd > out.log 2>&1
来源：http://bbl.yangfankeji.com

[R40] 追加写日志
来源：http://kql.chenzaomai.com

echo "log" >> out.log
来源：http://ekq.jinghuilouyu.cn

[R41] 丢弃输出
来源：http://jzh.xylfe.cn

cmd >/dev/null 2>&1
来源：http://fwf.iojbl.cn

[R42] 输入重定向
来源：http://tim.pengpengdd.cyou

wc -l < a.txt
来源：http://uqm.pycfn.com

[R43] 按名字查找文件
来源：http://bmc.jqgufenzy.top

find . -name "*.log" -type f
来源：http://bpq.zhongyouzk.top

[R44] 按修改时间查找
来源：http://mvk.quarkkingdee.top

find . -mtime -7 -type f
来源：http://xrx.zhoulong.xyz

[R45] 批量删除
来源：http://sfi.havefunace.top

find . -name "*.tmp" -delete
来源：http://mdf.yongpay.top

[R46] 递归替换文件内容
来源：http://ije.jianghu66.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xni.sjlbkw.cn

[R47] sed 单行替换
来源：http://dsj.svipenyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jqq.fzhhl.top

[R48] awk 取指定列
来源：http://yba.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://isv.tanke756.top

[R49] awk 带条件
来源：http://ymy.shzxlz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jtv.ybcxt.top

[R50] awk 求和
来源：http://nfe.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://lke.daria6918.cn

[R51] 排序去重取前几
来源：http://zhn.yanxiufei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xsb.wangshuangyany.cn

[R52] 统计行数
来源：http://zmy.ybcxt.top

wc -l a.txt
来源：http://zzj.bjfxy.top

[R53] 查看文件头与实时尾
来源：http://fvo.chenjidiqi.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://upd.shuidangran.top

[R54] 比较两个文件
来源：http://cix.xingfuxueyuan.xyz

diff a.txt b.txt
来源：http://sxm.yvedp.cn

[R55] 压缩与解压
来源：http://dup.yangfankeji.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jga.zdbjq.cn

[R56] 远程拷贝
来源：http://ajz.nanxuanxn.top

scp file user@host:/path/
来源：http://gue.tian-w.cn

[R57] 远程执行命令
来源：http://ezk.jyoumei.cn

ssh user@host 'uptime'
来源：http://jlq.uphjek.com

[R58] 下载文件
来源：http://nma.ctjpmb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yde.shuidangran.top

[R59] 发 POST JSON
来源：http://vle.ybcxt.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lxc.aizwys.cn

[R60] 只看 HTTP 状态码
来源：http://oer.jyoumei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zis.jqgufenzy.top

[R61] 磁盘占用
来源：http://cie.jlsjyb.cn

df -h;  du -sh *
来源：http://eim.sjlbkw.cn

[R62] 找最占空间的文件
来源：http://nzf.jinqigufen.top

du -ah . | sort -rh | head -10
来源：http://vxw.zdqjudy.top

[R63] 内存与进程
来源：http://ulm.ehwqpu.com

free -h;  ps aux | grep nginx
来源：http://xdc.zycfv.cn

[R64] 结束进程
来源：http://bix.fehbvm.com

kill -9 $(pgrep -f app.py)
来源：http://bzi.jlsjyb.cn

[R65] 查看端口占用
来源：http://hiz.yanxiufei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yfh.sxryk.cn

[R66] 定时任务
来源：http://kwx.xinyue.icu

crontab -e;  crontab -l
来源：http://xzh.hnqzz.top

[R67] 生成随机十六进制串
来源：http://von.uphjek.com

openssl rand -hex 16
来源：http://acu.jinyuanbaomall.cn

[R68] 计算文件校验值
来源：http://kom.vqdsnc.cn

sha256sum a.txt;  md5sum a.txt
来源：http://axe.ybcxt.top

[R69] 生成随机密码
来源：http://uyf.zhiwuduotai.top

head -c 16 /dev/urandom | base64
来源：http://tln.ehwqpu.com

[R70] 时间戳与互转
来源：http://ujp.yangfankeji.com

date +%s;  date -d @1700000000
来源：http://zsr.fanxiaobao.xyz

[R71] 日期格式化
来源：http://bwp.hesvh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qlx.wangshuangyany.cn

[R72] 等待端口就绪
来源：http://psy.hongshengwenyu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://svh.epnwcf.com

[R73] 分割大日志
来源：http://tko.hcnkem.com

split -l 1000 big.log part_
来源：http://edn.dashuyun.cn

[R74] 批量重命名
来源：http://blw.tian-w.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://awt.gaohongyu789.top

[R75] 导出环境变量
来源：http://wor.snrcjt.cn

export PATH="$HOME/bin:$PATH"
来源：http://ycu.yfazqb.com

[R76] 使用临时文件
来源：http://cpu.guannengcc.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xdt.gzhubu.top

[R77] 读取用户输入
来源：http://efk.0kj1m.cn

read -rp "请输入: " ans
来源：http://skk.xuanzx.com

[R78] 交互式菜单
来源：http://amq.shanyushiyangtech.top

select opt in a b c; do echo "$opt"; break; done
来源：http://crk.zhixingplan.top

[R79] 解析命令行选项
来源：http://fdy.zhiwuduotai.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ygg.0kj1m.cn

[R80] 查看脚本执行耗时
来源：http://abw.shuidangran.top

time ./run.sh
来源：http://cml.jlsjyb.cn

================================================================================
来源：http://goa.shuidangran.top

S. C / C++ 专题
来源：http://oih.chenjidiqi.icu

================================================================================
来源：http://yvd.dashuyun.cn

[S01] C：Hello World
来源：http://zdf.ivvv.top

#include <stdio.h>
来源：http://bnv.feifeiyinyue.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gau.hesvh.cn

[S02] C：变量与格式化输出
来源：http://zrf.zhaomingkeji.xyz

int a = 10; printf("%d\n", a);
来源：http://xqs.dashuyun.cn

[S03] C：读入整数
来源：http://gzy.fanxiaobao.xyz

int x; scanf("%d", &x);
来源：http://ezq.fktsv.cn

[S04] C：字符串复制
来源：http://ixi.jqgfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://znx.shanyushiyangtech.top

[S05] C：字符串长度
来源：http://key.xylfe.cn

strlen(s)
来源：http://yfc.yangfankeji.com

[S06] C：字符串比较
来源：http://jve.nanxuanxn.top

strcmp(a, b) == 0
来源：http://raw.c1oappe.top

[S07] C：数组遍历求和
来源：http://urr.mhx1999.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uez.xziqi.cn

[S08] C：动态内存分配与释放
来源：http://oze.chenjidiqi.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oyc.iojbl.cn

[S09] C：结构体定义与初始化
来源：http://pxf.zhaomingkeji.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://joh.nwbrower.top

[S10] C：指针与解引用
来源：http://iay.fengsongda.top

int *p = &a;  *p = 5;
来源：http://llq.andypj.xyz

[S11] C：逐行读文件
来源：http://kxd.bbcook.cn

FILE *f = fopen("a.txt", "r");
来源：http://jkn.sweek.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ngc.gotoacloud.top

fclose(f);
来源：http://fig.fzhhl.top

[S12] C：写文件
来源：http://vcc.fzhhl.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xvz.cashguo.top

[S13] C：宏定义
来源：http://tla.c1oappe.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kzd.zdbjq.cn

[S14] C：枚举
来源：http://vzo.jqgufenzy.top

enum Color { RED, GREEN, BLUE };
来源：http://vme.tanke756.top

[S15] C：类型转换
来源：http://ylt.ivvv.top

(double) a / b
来源：http://bex.yonumen.top

[S16] C：位操作置位
来源：http://epp.hcnkem.com

x |= (1 << 3);
来源：http://maf.jiagoushi.top

[S17] C：安全拼接字符串
来源：http://dhx.yvedp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kvr.tianlin.xyz

[S18] C：命令行参数
来源：http://dhk.cucudq.cn

int main(int argc, char **argv)
来源：http://nzh.shuidangran.top

[S19] C：快速排序
来源：http://ubk.jianghu66.top

qsort(a, n, sizeof(int), cmp);
来源：http://vnl.redwolf501.top

[S20] C：二分查找
来源：http://pbt.yj202588.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ffr.hnxiangtu.top

[S21] C：字符类别判断
来源：http://lib.xuanzx.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://czs.xingfuxueyuan.xyz

[S22] C：字符串转数字
来源：http://njm.nanxuanxn.top

atoi("42");  strtod("3.14", NULL);
来源：http://duw.jlsjyb.cn

[S23] C：随机数
来源：http://tsa.dashuyun.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bnc.hongshengwenyu.top

[S24] C：获取本地时间
来源：http://asx.uphjek.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://typ.ppjwa.cn

[S25] C：内存拷贝
来源：http://pro.mhx1999.top

memcpy(dst, src, n);
来源：http://acp.nanxinkj.top

[S26] C：内存清零
来源：http://pky.nwbrower.top

memset(a, 0, sizeof a);
来源：http://inn.epnwcf.com

[S27] C：定义常量
来源：http://kqt.fehbvm.com

const double PI = 3.14159;
来源：http://prb.bbcook.cn

[S28] C：静态变量
来源：http://xby.sysykeji.top

static int counter = 0;
来源：http://uyj.jqgfzy.top

[S29] C：变参函数
来源：http://zio.sysykeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pdm.yanxiufei.cn

[S30] C：头文件保护
来源：http://spw.ybcxt.top

#ifndef X_H
来源：http://avf.vqdsnc.cn

#define X_H
来源：http://nxh.shanyushiyangtech.top

#endif
来源：http://lsm.yueranfly.top

[S31] C++：Hello World
来源：http://fiy.jinghuilouyu.cn

#include <iostream>
来源：http://ujb.yueranfly.top

int main() { std::cout << "Hello\n"; }
来源：http://ied.bbcook.cn

[S32] C++：字符串
来源：http://mta.guannengcc.top

std::string s = "hi";  s += "!";
来源：http://rhe.havefunace.top

[S33] C++：vector 增删
来源：http://qfr.aibaodan.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pfq.c1oappe.top

[S34] C++：遍历 vector
来源：http://dbj.sjlbkw.cn

for (auto &x : v) { std::cout << x; }
来源：http://ozb.zhiwuduotai.top

[S35] C++：map
来源：http://tti.aizwys.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hsa.mhx1999.top

[S36] C++：unordered_map
来源：http://mzq.uphjek.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yat.pycfn.com

[S37] C++：set
来源：http://jry.havefunace.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zvd.yuanzhike.top

[S38] C++：排序
来源：http://ghu.havefunace.top

std::sort(v.begin(), v.end());
来源：http://xvn.zhixingplan.top

[S39] C++：自定义比较器排序
来源：http://rao.haohaochexian.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dzu.jyoumei.cn

[S40] C++：查找元素
来源：http://vwr.dianchejie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gmn.nanxuanxn.top

[S41] C++：类与构造函数
来源：http://tsl.hnxiangtu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nmp.zhaomingkeji.xyz

[S42] C++：继承与虚函数
来源：http://jvj.hammf.cn

class B : public Base { public: void f() override {} };
来源：http://ttd.yonumen.top

[S43] C++：智能指针
来源：http://mws.shzxlz.cn

auto p = std::make_unique<int>(5);
来源：http://wof.shuidangran.top

[S44] C++：引用传参
来源：http://yxw.tarul.cn

void inc(int &x) { ++x; }
来源：http://mpz.hcnkem.com

[S45] C++：lambda
来源：http://wnw.svipenyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rjy.kuanghao11.cn

[S46] C++：函数模板
来源：http://lfb.daxiang520.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ptp.yonumen.top

[S47] C++：结构化绑定遍历
来源：http://lmw.jianghu66.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pvc.pycfn.com

[S48] C++：逐行读文件
来源：http://kqf.dianchejie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sfu.zhijiandao.cn

while (std::getline(in, line)) { }
来源：http://ufq.zycfv.cn

[S49] C++：写文件
来源：http://sih.yuanzhike.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zxb.pengpengdd.cyou

[S50] C++：格式化数字
来源：http://sev.ivvv.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lvj.sysykeji.top

[S51] C++：显式类型转换
来源：http://xeu.tarul.cn

static_cast<double>(a) / b
来源：http://xhd.jyoumei.cn

[S52] C++：const 与 noexcept
来源：http://muh.xylfe.cn

int size() const noexcept { return n_; }
来源：http://lkk.chenjidiqi.icu

[S53] C++：移动语义
来源：http://jie.bbcook.cn

std::vector<int> w = std::move(v);
来源：http://mok.fktsv.cn

[S54] C++：异常处理
来源：http://cwq.hesvh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pnu.vqdsnc.cn

[S55] C++：结构化绑定
来源：http://wru.cqqwz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tgx.0kj1m.cn

[S56] C++：optional
来源：http://frt.yj202588.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kog.andypj.xyz

[S57] C++：编译期常量
来源：http://rtp.yanxiufei.cn

constexpr int N = 10;
来源：http://csg.zdqjudy.top

[S58] C++：命名空间
来源：http://qji.zhixingplan.top

namespace ns { int f() { return 1; } }
来源：http://yuq.cqqwz.cn

[S59] C++：静态断言
来源：http://xfb.ctjpmb.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zwh.sxryk.cn

[S60] C++：遍历并删除元素
来源：http://mrr.ivvv.top


<!-- 参考信息 -->