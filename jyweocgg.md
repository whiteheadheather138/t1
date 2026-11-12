代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bzo.jinqigfzy.top

[Q90] 生成序号列
来源：http://vvx.chenlongwang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tbs.fanxiaobao.xyz

================================================================================
来源：http://usq.hongshengwenyu.top

R. Bash 专题
来源：http://kay.haohaochexian.top

================================================================================
来源：http://spv.chenlongwang.top

[R01] shebang 与严格模式
来源：http://wob.tarul.cn

#!/usr/bin/env bash
来源：http://rze.zdqjudy.top

set -euo pipefail
来源：http://sng.ydzc1.top

[R02] 变量赋值与使用
来源：http://nxq.cashguo.top

name="Tom"; echo "$name"
来源：http://wea.cqqwz.cn

[R03] 只读变量
来源：http://gvj.xylfe.cn

readonly PI=3.14
来源：http://nvb.jiagoushi.top

[R04] 位置参数
来源：http://fmx.uphjek.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nyf.yvedp.cn

[R05] 参数默认值
来源：http://uic.shanyushiyangkeji.top

name="${1:-default}"
来源：http://mkl.tian-w.cn

[R06] 判断命令是否存在
来源：http://lok.haohaochexian.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sxg.smart0.xyz

[R07] if 判断文件
来源：http://tri.jinqigufen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mhq.xinyue.icu

[R08] 数值比较
来源：http://klq.mhx1999.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nrc.xylfe.cn

[R09] 字符串比较
来源：http://mns.smart0.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fac.9152youxi.cn

[R10] 正则匹配
来源：http://zri.sweek.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rob.ybcxt.top

[R11] case 多分支
来源：http://tqn.zhaomingkeji.xyz

case "$1" in
来源：http://tbc.yfazqb.com

start) echo "启动" ;;
来源：http://isy.zycfv.cn

stop)  echo "停止" ;;
来源：http://jor.fanxiaobao.xyz

*)     echo "未知命令" ;;
来源：http://epv.yj20258888.top

esac
来源：http://osa.yonumen.top

[R12] for 遍历文件
来源：http://zds.ybcxt.top

for f in *.txt; do echo "$f"; done
来源：http://vwg.chenjidiqi.icu

[R13] for 计数循环
来源：http://bum.shangyingyoupin.top

for i in {1..10}; do echo "$i"; done
来源：http://zzf.zhoulong.xyz

[R14] C 风格 for
来源：http://vep.zhaomingkeji.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qhi.jinqigufen.top

[R15] while 逐行读文件
来源：http://icg.haohaochexian.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xct.yongpay.top

[R16] until 等待条件
来源：http://hmc.iojbl.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://csv.zycfv.cn

[R17] 数组定义与取值
来源：http://gns.nanxinkj.top

arr=(a b c); echo "${arr[0]}"
来源：http://mky.gogol.net.cn

[R18] 遍历数组
来源：http://ixi.ehwqpu.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wle.wangdashe.top

[R19] 数组长度
来源：http://zfa.zhixingplan.top

echo "${#arr[@]}"
来源：http://ltj.pycfn.com

[R20] 关联数组（字典）
来源：http://umm.ctjpmb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hoi.c1oappe.top

[R21] 字符串长度
来源：http://wvc.zdqjudy.top

echo "${#s}"
来源：http://byc.iojbl.cn

[R22] 截取子串
来源：http://qub.aibaodan.cn

echo "${s:0:5}"
来源：http://jeh.hongshengwenyu.top

[R23] 字符串替换
来源：http://pop.zdbjq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sxi.jqgfzy.top

[R24] 大小写转换
来源：http://jsq.uphjek.com

echo "${s^^}"; echo "${s,,}"
来源：http://esy.c1oappe.top

[R25] 去后缀 / 去前缀
来源：http://san.hesvh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://deo.dashuyun.cn

[R26] 命令替换
来源：http://faa.hesvh.cn

now=$(date +%F); echo "$now"
来源：http://fap.nwbrower.top

[R27] 算术展开
来源：http://hmx.hcnkem.com

echo $((1 + 2 * 3))
来源：http://tua.hongshengwenyu.top

[R28] 浮点运算
来源：http://xvf.daxiang520.top

echo "scale=2; 10/3" | bc
来源：http://uer.sjlbkw.cn

[R29] 定义函数
来源：http://wlh.meibo888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://urx.jianghu66.top

[R30] 函数返回状态码
来源：http://uiv.xingfuxueyuan.xyz

f() { return 0; }; f || echo "失败了"
来源：http://tht.cqqwz.cn

[R31] 局部变量
来源：http://lor.zdqjudy.top

f() { local x=1; echo "$x"; }
来源：http://orw.hnxiangtu.top

[R32] 参数个数校验
来源：http://nmg.gzhubu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wsw.jinyuanbaomall.cn

[R33] 捕获错误并提示行号
来源：http://fot.shangyingyoupin.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ffx.jinghuilouyu.cn

[R34] 退出时清理
来源：http://wcy.ydjk.org.cn

trap 'rm -f "$tmp"' EXIT
来源：http://iwd.xuetiantiany.cn

[R35] 后台执行并等待
来源：http://olz.ivvv.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jbb.yueranfly.top

[R36] 并发执行多个任务
来源：http://rzb.birdmap.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hju.cqqwz.cn

[R37] 把输出赋给变量
来源：http://ffh.vqdsnc.cn

files=$(ls -1)
来源：http://cps.tarul.cn

[R38] 管道串联
来源：http://yfc.daria6918.cn

cat a.txt | grep -i error | wc -l
来源：http://pzy.uphjek.com

[R39] 重定向标准输出与错误
来源：http://lnb.gzhubu.top

cmd > out.log 2>&1
来源：http://qfx.chenzaomai.com

[R40] 追加写日志
来源：http://efc.gzhubu.top

echo "log" >> out.log
来源：http://mvy.yonumen.top

[R41] 丢弃输出
来源：http://kdh.chenzaomai.com

cmd >/dev/null 2>&1
来源：http://svb.9152youxi.cn

[R42] 输入重定向
来源：http://hzo.jinqigufen.top

wc -l < a.txt
来源：http://gvd.cqqwz.cn

[R43] 按名字查找文件
来源：http://qlg.fengsongda.top

find . -name "*.log" -type f
来源：http://vrz.hnqzz.top

[R44] 按修改时间查找
来源：http://zvk.meibo888.top

find . -mtime -7 -type f
来源：http://oap.snrcjt.cn

[R45] 批量删除
来源：http://peg.redwolf501.top

find . -name "*.tmp" -delete
来源：http://vfa.ydzc1.top

[R46] 递归替换文件内容
来源：http://sng.fehbvm.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cap.xuanzx.com

[R47] sed 单行替换
来源：http://lrg.fengsongda.top

sed -i 's/foo/bar/g' a.txt
来源：http://doe.cashguo.top

[R48] awk 取指定列
来源：http://okx.zhoulong.xyz

awk '{print $1, $3}' a.txt
来源：http://bxe.cheryme.top

[R49] awk 带条件
来源：http://mtw.zhijiandao.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blx.vqdsnc.cn

[R50] awk 求和
来源：http://gaa.aizwys.cn

awk '{s += $2} END {print s}' a.txt
来源：http://woi.jqgufenzy.top

[R51] 排序去重取前几
来源：http://aye.hywenlv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ojz.ydjk.org.cn

[R52] 统计行数
来源：http://kum.0kj1m.cn

wc -l a.txt
来源：http://vwd.snrcjt.cn

[R53] 查看文件头与实时尾
来源：http://rtg.nwbrower.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://arq.yangfankeji.com

[R54] 比较两个文件
来源：http://apd.daria6918.cn

diff a.txt b.txt
来源：http://yzp.daxiang520.top

[R55] 压缩与解压
来源：http://ect.nanxinkj.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mjb.kuanghao11.cn

[R56] 远程拷贝
来源：http://xiq.zycfv.cn

scp file user@host:/path/
来源：http://lpd.sweek.top

[R57] 远程执行命令
来源：http://fav.aibaodan.cn

ssh user@host 'uptime'
来源：http://sxi.guowangkeji.top

[R58] 下载文件
来源：http://ooq.quarkkingdee.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://amj.shzxlz.cn

[R59] 发 POST JSON
来源：http://dxd.kuanghao11.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eis.0kj1m.cn

[R60] 只看 HTTP 状态码
来源：http://zdf.redwolf501.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dsw.jqgfzy.top

[R61] 磁盘占用
来源：http://hjj.mhx1999.top

df -h;  du -sh *
来源：http://yzb.hongshengwenyu.top

[R62] 找最占空间的文件
来源：http://ptm.sweek.top

du -ah . | sort -rh | head -10
来源：http://otl.jqgufenzy.top

[R63] 内存与进程
来源：http://oqk.jyoumei.cn

free -h;  ps aux | grep nginx
来源：http://mma.yvedp.cn

[R64] 结束进程
来源：http://fwt.hfpthk.cn

kill -9 $(pgrep -f app.py)
来源：http://rxg.zhaomingkeji.xyz

[R65] 查看端口占用
来源：http://whh.jinqigufen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tbp.jianghu66.top

[R66] 定时任务
来源：http://hki.xziqi.cn

crontab -e;  crontab -l
来源：http://sst.svipenyu.cn

[R67] 生成随机十六进制串
来源：http://pta.smart0.xyz

openssl rand -hex 16
来源：http://rej.0kj1m.cn

[R68] 计算文件校验值
来源：http://sev.fengsongda.top

sha256sum a.txt;  md5sum a.txt
来源：http://dkh.jqgufenzy.top

[R69] 生成随机密码
来源：http://plu.zhixingplan.top

head -c 16 /dev/urandom | base64
来源：http://gyv.fktsv.cn

[R70] 时间戳与互转
来源：http://xit.nanxinkj.top

date +%s;  date -d @1700000000
来源：http://tcs.jinghuilouyu.cn

[R71] 日期格式化
来源：http://pre.zdqjudy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ifi.snrcjt.cn

[R72] 等待端口就绪
来源：http://oxn.andypj.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://xzr.ppjwa.cn

[R73] 分割大日志
来源：http://jdw.cdnleiting.top

split -l 1000 big.log part_
来源：http://vub.gaohongyu789.top

[R74] 批量重命名
来源：http://orf.gzhubu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://idi.52xcode.cn

[R75] 导出环境变量
来源：http://tnb.yj202588.top

export PATH="$HOME/bin:$PATH"
来源：http://wuk.316326.xyz

[R76] 使用临时文件
来源：http://gbq.tanke756.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fsg.zycfv.cn

[R77] 读取用户输入
来源：http://jkd.zdbjq.cn

read -rp "请输入: " ans
来源：http://iyt.sxryk.cn

[R78] 交互式菜单
来源：http://lyx.bbcook.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uca.zdbjq.cn

[R79] 解析命令行选项
来源：http://pwa.fktsv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ftw.tian-w.cn

[R80] 查看脚本执行耗时
来源：http://cgy.nanxinkj.top

time ./run.sh
来源：http://mxg.zdbjq.cn

================================================================================
来源：http://yox.smart0.xyz

S. C / C++ 专题
来源：http://kiy.shzxlz.cn

================================================================================
来源：http://crh.pycfn.com

[S01] C：Hello World
来源：http://teu.52xcode.cn

#include <stdio.h>
来源：http://jmu.aibaodan.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gkn.shzxlz.cn

[S02] C：变量与格式化输出
来源：http://rxr.ivvv.top

int a = 10; printf("%d\n", a);
来源：http://oox.zycfv.cn

[S03] C：读入整数
来源：http://hjk.gotoacloud.top

int x; scanf("%d", &x);
来源：http://tge.shzxlz.cn

[S04] C：字符串复制
来源：http://cxs.cqqwz.cn

char dst[32]; strcpy(dst, "hi");
来源：http://scu.vehdjk.com

[S05] C：字符串长度
来源：http://lab.snrcjt.cn

strlen(s)
来源：http://wra.bjfxy.top

[S06] C：字符串比较
来源：http://kfv.sufxvd.cn

strcmp(a, b) == 0
来源：http://rpi.aizwys.cn

[S07] C：数组遍历求和
来源：http://zof.yvedp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vft.yanxiufei.cn

[S08] C：动态内存分配与释放
来源：http://dxf.jiagoushi.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://khz.andypj.xyz

[S09] C：结构体定义与初始化
来源：http://qxb.yuxming.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uiq.daria6918.cn

[S10] C：指针与解引用
来源：http://uhp.tianlin.xyz

int *p = &a;  *p = 5;
来源：http://ufx.kuanghao11.cn

[S11] C：逐行读文件
来源：http://bdh.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "r");
来源：http://gbv.jinghuilouyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gen.gzhubu.top

fclose(f);
来源：http://eqy.wangshuangyany.cn

[S12] C：写文件
来源：http://gqe.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jon.kuanghao11.cn

[S13] C：宏定义
来源：http://xhu.xuetiantiany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hin.ydzc1.top

[S14] C：枚举
来源：http://soz.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://mjo.hysaishi.cn

[S15] C：类型转换
来源：http://dqm.0kj1m.cn

(double) a / b
来源：http://dox.gotoacloud.top

[S16] C：位操作置位
来源：http://ink.hammf.cn

x |= (1 << 3);
来源：http://xyv.yj202588.top

[S17] C：安全拼接字符串
来源：http://djo.redwolf501.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://keq.zhixingplan.top

[S18] C：命令行参数
来源：http://wmq.cheryme.top

int main(int argc, char **argv)
来源：http://ojw.wangdashe.top

[S19] C：快速排序
来源：http://whn.c1oappe.top

qsort(a, n, sizeof(int), cmp);
来源：http://zyu.cqqwz.cn

[S20] C：二分查找
来源：http://ivx.wangshuangyany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oby.chenzaomai.com

[S21] C：字符类别判断
来源：http://otz.yvedp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pis.zdqjudy.top

[S22] C：字符串转数字
来源：http://hke.fanxiaobao.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://vjm.gaohongyu789.top

[S23] C：随机数
来源：http://ode.hywenlv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vfc.yuanzhike.top

[S24] C：获取本地时间
来源：http://qeo.xingfuxueyuan.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yrn.snrcjt.cn

[S25] C：内存拷贝
来源：http://sjc.sysykeji.top

memcpy(dst, src, n);
来源：http://ish.hfpthk.cn

[S26] C：内存清零
来源：http://kka.ctjpmb.com

memset(a, 0, sizeof a);
来源：http://iug.feifeiyinyue.top

[S27] C：定义常量
来源：http://gju.c1oappe.top

const double PI = 3.14159;
来源：http://rtp.sweek.top

[S28] C：静态变量
来源：http://etw.chenzaomai.com

static int counter = 0;
来源：http://kxu.epnwcf.com

[S29] C：变参函数
来源：http://obm.jinghuilouyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mxl.wangdashe.top

[S30] C：头文件保护
来源：http://qub.jqgfzy.top

#ifndef X_H
来源：http://qea.tarul.cn

#define X_H
来源：http://sgo.zhijiandao.cn

#endif
来源：http://nii.shanyushiyangtech.top

[S31] C++：Hello World
来源：http://vli.andypj.xyz

#include <iostream>
来源：http://rnl.chenjidiqi.icu

int main() { std::cout << "Hello\n"; }
来源：http://byu.daria6918.cn

[S32] C++：字符串
来源：http://yur.jyoumei.cn

std::string s = "hi";  s += "!";
来源：http://kch.cheryme.top

[S33] C++：vector 增删
来源：http://sjd.haohaochexian.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ddo.nwbrower.top

[S34] C++：遍历 vector
来源：http://eom.guowangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://zhy.yongpay.top

[S35] C++：map
来源：http://xzr.zhixingplan.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xrm.shangyingyoupin.top

[S36] C++：unordered_map
来源：http://crv.zhengqikj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zwp.daxiang520.top

[S37] C++：set
来源：http://spe.hesvh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bxw.cqqwz.cn

[S38] C++：排序
来源：http://zbz.nanxinkj.top

std::sort(v.begin(), v.end());
来源：http://otw.sysykeji.top

[S39] C++：自定义比较器排序
来源：http://mwp.pengpengdd.cyou

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://igt.ydjk.org.cn

[S40] C++：查找元素
来源：http://xjz.mhx1999.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dnc.xylfe.cn

[S41] C++：类与构造函数
来源：http://oxh.feifeiyinyue.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rpi.tarul.cn

[S42] C++：继承与虚函数
来源：http://kse.uphjek.com

class B : public Base { public: void f() override {} };
来源：http://nel.dashuyun.cn

[S43] C++：智能指针
来源：http://wgn.c1oappe.top

auto p = std::make_unique<int>(5);
来源：http://voa.vqdsnc.cn

[S44] C++：引用传参
来源：http://gtl.yueranfly.top

void inc(int &x) { ++x; }
来源：http://gft.yueranfly.top

[S45] C++：lambda
来源：http://ltz.aibaodan.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dwk.zdbjq.cn

[S46] C++：函数模板
来源：http://phi.shangyingyoupin.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jue.yj20258888.top

[S47] C++：结构化绑定遍历
来源：http://azx.ehwqpu.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://llk.ybcxt.top

[S48] C++：逐行读文件
来源：http://zhh.yuxming.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nor.redwolf501.top

while (std::getline(in, line)) { }
来源：http://tzv.jinqigfzy.top

[S49] C++：写文件
来源：http://aqk.mhx1999.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hqg.aibaodan.cn

[S50] C++：格式化数字
来源：http://wvi.chenjidiqi.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gqg.cucudq.cn

[S51] C++：显式类型转换
来源：http://vml.yj202588.top

static_cast<double>(a) / b
来源：http://wmt.zhixingplan.top

[S52] C++：const 与 noexcept
来源：http://zkv.zhijiandao.cn

int size() const noexcept { return n_; }
来源：http://uzo.hammf.cn

[S53] C++：移动语义
来源：http://pwz.chenjidiqi.icu

std::vector<int> w = std::move(v);
来源：http://ksi.yuxming.cn

[S54] C++：异常处理
来源：http://fvp.yj20258888.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://guf.vqdsnc.cn

[S55] C++：结构化绑定
来源：http://axg.xinyue.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://ftc.bjfxy.top

[S56] C++：optional
来源：http://wdp.shanyushiyangtech.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xqo.hcnkem.com

[S57] C++：编译期常量
来源：http://bom.hnxiangtu.top

constexpr int N = 10;
来源：http://aah.nanxuanxn.top

[S58] C++：命名空间
来源：http://ouz.hnxiangtu.top

namespace ns { int f() { return 1; } }
来源：http://asl.nwbrower.top

[S59] C++：静态断言
来源：http://vzq.jinqigufen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ejj.sxryk.cn

[S60] C++：遍历并删除元素
来源：http://qhx.ydzc1.top


<!-- 参考信息 -->