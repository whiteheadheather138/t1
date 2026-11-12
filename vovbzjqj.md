代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mbi.cucudq.cn

[Q90] 生成序号列
来源：http://cha.jlsjyb.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://imm.yfazqb.com

================================================================================
来源：http://xtq.shanyushiyangtech.top

R. Bash 专题
来源：http://wix.wangshuangyany.cn

================================================================================
来源：http://rlh.vehdjk.com

[R01] shebang 与严格模式
来源：http://tty.zhengqikj.top

#!/usr/bin/env bash
来源：http://tap.nanxinkj.top

set -euo pipefail
来源：http://eas.sufxvd.cn

[R02] 变量赋值与使用
来源：http://vbb.yj20258.top

name="Tom"; echo "$name"
来源：http://spi.c1oappe.top

[R03] 只读变量
来源：http://eio.fehbvm.com

readonly PI=3.14
来源：http://qqq.svipenyu.cn

[R04] 位置参数
来源：http://oty.redwolf501.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dkw.sufxvd.cn

[R05] 参数默认值
来源：http://pgo.hcnkem.com

name="${1:-default}"
来源：http://icp.chenzaomai.com

[R06] 判断命令是否存在
来源：http://ocb.hywenlv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vna.svipenyu.cn

[R07] if 判断文件
来源：http://zbe.tianlin.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mng.fengsongda.top

[R08] 数值比较
来源：http://ryk.wangshuangyany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vqk.kuanghao11.cn

[R09] 字符串比较
来源：http://wfs.gzhubu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hqj.zhoulong.xyz

[R10] 正则匹配
来源：http://uzs.jianghu66.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tzl.bbcook.cn

[R11] case 多分支
来源：http://dcl.gzhubu.top

case "$1" in
来源：http://bmz.pengpengdd.cyou

start) echo "启动" ;;
来源：http://ape.52xcode.cn

stop)  echo "停止" ;;
来源：http://ous.bjfxy.top

*)     echo "未知命令" ;;
来源：http://cay.jqgufenzy.top

esac
来源：http://ypf.yfazqb.com

[R12] for 遍历文件
来源：http://uke.ydzc1.top

for f in *.txt; do echo "$f"; done
来源：http://kdc.zhengqikj.top

[R13] for 计数循环
来源：http://mwq.hfpthk.cn

for i in {1..10}; do echo "$i"; done
来源：http://dfi.xylfe.cn

[R14] C 风格 for
来源：http://izy.birdmap.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://faw.cashguo.top

[R15] while 逐行读文件
来源：http://jbp.hysaishi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pyw.pycfn.com

[R16] until 等待条件
来源：http://fnj.gzhubu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bnu.yueranfly.top

[R17] 数组定义与取值
来源：http://wlo.jinqigfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://uwr.jyoumei.cn

[R18] 遍历数组
来源：http://uyr.gzhubu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xau.xuanzx.com

[R19] 数组长度
来源：http://hbj.feifeiyinyue.top

echo "${#arr[@]}"
来源：http://ptv.jlsjyb.cn

[R20] 关联数组（字典）
来源：http://qtx.hesvh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ffi.cdnleiting.top

[R21] 字符串长度
来源：http://ywp.xingfuxueyuan.xyz

echo "${#s}"
来源：http://tgh.daria6918.cn

[R22] 截取子串
来源：http://lqc.guowangkeji.top

echo "${s:0:5}"
来源：http://rup.vehdjk.com

[R23] 字符串替换
来源：http://gdp.feifeiyinyue.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vft.uphjek.com

[R24] 大小写转换
来源：http://iqq.zhaomingkeji.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://njs.daria6918.cn

[R25] 去后缀 / 去前缀
来源：http://uej.cashguo.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jmi.tanke756.top

[R26] 命令替换
来源：http://cku.yuanzhike.top

now=$(date +%F); echo "$now"
来源：http://qur.yuanzhike.top

[R27] 算术展开
来源：http://elc.nanxinkj.top

echo $((1 + 2 * 3))
来源：http://pvt.quarkkingdee.top

[R28] 浮点运算
来源：http://fkj.ydjk.org.cn

echo "scale=2; 10/3" | bc
来源：http://fxr.shzxlz.cn

[R29] 定义函数
来源：http://vsx.ehwqpu.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hjk.zycfv.cn

[R30] 函数返回状态码
来源：http://ids.hfpthk.cn

f() { return 0; }; f || echo "失败了"
来源：http://tvq.dashuyun.cn

[R31] 局部变量
来源：http://ycv.xylfe.cn

f() { local x=1; echo "$x"; }
来源：http://aue.yvedp.cn

[R32] 参数个数校验
来源：http://vgl.yongpay.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pcp.gotoacloud.top

[R33] 捕获错误并提示行号
来源：http://spw.yanxiufei.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ppj.zhiwuduotai.top

[R34] 退出时清理
来源：http://exp.hnqzz.top

trap 'rm -f "$tmp"' EXIT
来源：http://jym.bjfxy.top

[R35] 后台执行并等待
来源：http://jcn.epnwcf.com

sleep 5 & pid=$!; wait "$pid"
来源：http://pbz.jianghu66.top

[R36] 并发执行多个任务
来源：http://ywr.cucudq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qpw.andypj.xyz

[R37] 把输出赋给变量
来源：http://hgj.nanxinkj.top

files=$(ls -1)
来源：http://skv.svipenyu.cn

[R38] 管道串联
来源：http://pwx.zhiwuduotai.top

cat a.txt | grep -i error | wc -l
来源：http://xce.chenlongwang.top

[R39] 重定向标准输出与错误
来源：http://iry.gzhubu.top

cmd > out.log 2>&1
来源：http://luv.wangshuangyany.cn

[R40] 追加写日志
来源：http://afc.jinqigufen.top

echo "log" >> out.log
来源：http://bwm.shanyushiyangtech.top

[R41] 丢弃输出
来源：http://pct.tanke756.top

cmd >/dev/null 2>&1
来源：http://fyl.tianlin.xyz

[R42] 输入重定向
来源：http://ope.ppjwa.cn

wc -l < a.txt
来源：http://jzh.aibaodan.cn

[R43] 按名字查找文件
来源：http://ofi.sysykeji.top

find . -name "*.log" -type f
来源：http://ubj.yonumen.top

[R44] 按修改时间查找
来源：http://nfq.xingfuxueyuan.xyz

find . -mtime -7 -type f
来源：http://caa.daria6918.cn

[R45] 批量删除
来源：http://wdh.yj20258888.top

find . -name "*.tmp" -delete
来源：http://lns.zhijiandao.cn

[R46] 递归替换文件内容
来源：http://eib.guannengcc.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://flj.aibaodan.cn

[R47] sed 单行替换
来源：http://muu.c1oappe.top

sed -i 's/foo/bar/g' a.txt
来源：http://kfl.jqgufenzy.top

[R48] awk 取指定列
来源：http://fjq.zhixingplan.top

awk '{print $1, $3}' a.txt
来源：http://zkj.xylfe.cn

[R49] awk 带条件
来源：http://nws.dashuyun.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://csc.hnxiangtu.top

[R50] awk 求和
来源：http://mzo.xylfe.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cbo.cheryme.top

[R51] 排序去重取前几
来源：http://xgh.chenzaomai.com

sort a.txt | uniq -c | sort -rn | head
来源：http://gld.tanke756.top

[R52] 统计行数
来源：http://nec.hnxiangtu.top

wc -l a.txt
来源：http://onz.sufxvd.cn

[R53] 查看文件头与实时尾
来源：http://vpf.gogol.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qqn.fanxiaobao.xyz

[R54] 比较两个文件
来源：http://aey.guowangkeji.top

diff a.txt b.txt
来源：http://oap.chenjidiqi.icu

[R55] 压缩与解压
来源：http://zsq.svipenyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dnv.zhengqikj.top

[R56] 远程拷贝
来源：http://sob.ybcxt.top

scp file user@host:/path/
来源：http://whx.chenjidiqi.icu

[R57] 远程执行命令
来源：http://ryg.yueranfly.top

ssh user@host 'uptime'
来源：http://zov.yj202588.top

[R58] 下载文件
来源：http://cem.sjlbkw.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zmm.yongpay.top

[R59] 发 POST JSON
来源：http://uez.pycfn.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hbw.smart0.xyz

[R60] 只看 HTTP 状态码
来源：http://lzc.sjlbkw.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nxs.fehbvm.com

[R61] 磁盘占用
来源：http://mdb.xziqi.cn

df -h;  du -sh *
来源：http://qhy.haohaochexian.top

[R62] 找最占空间的文件
来源：http://pao.aibaodan.cn

du -ah . | sort -rh | head -10
来源：http://ebr.ivvv.top

[R63] 内存与进程
来源：http://zjl.jyoumei.cn

free -h;  ps aux | grep nginx
来源：http://rty.wangshuangyany.cn

[R64] 结束进程
来源：http://prn.hongshengwenyu.top

kill -9 $(pgrep -f app.py)
来源：http://cla.shzxlz.cn

[R65] 查看端口占用
来源：http://qun.yuxming.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://etj.cashguo.top

[R66] 定时任务
来源：http://kdw.nanxinkj.top

crontab -e;  crontab -l
来源：http://owl.yongpay.top

[R67] 生成随机十六进制串
来源：http://pof.cheryme.top

openssl rand -hex 16
来源：http://wzl.aibaodan.cn

[R68] 计算文件校验值
来源：http://szc.yonumen.top

sha256sum a.txt;  md5sum a.txt
来源：http://udv.svipenyu.cn

[R69] 生成随机密码
来源：http://vfs.ydzc1.top

head -c 16 /dev/urandom | base64
来源：http://xvg.yanxiufei.cn

[R70] 时间戳与互转
来源：http://pss.daxiang520.top

date +%s;  date -d @1700000000
来源：http://tqn.nwbrower.top

[R71] 日期格式化
来源：http://jsg.snrcjt.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jwt.hywenlv.cn

[R72] 等待端口就绪
来源：http://pgr.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://wei.yanxiufei.cn

[R73] 分割大日志
来源：http://zsx.hcnkem.com

split -l 1000 big.log part_
来源：http://wqh.shangyingyoupin.top

[R74] 批量重命名
来源：http://alh.sjlbkw.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mrw.mhx1999.top

[R75] 导出环境变量
来源：http://lcy.chenlongwang.top

export PATH="$HOME/bin:$PATH"
来源：http://qqq.jinqigufen.top

[R76] 使用临时文件
来源：http://imr.kuanghao11.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://iiv.meibo888.top

[R77] 读取用户输入
来源：http://idt.c1oappe.top

read -rp "请输入: " ans
来源：http://tbm.tian-w.cn

[R78] 交互式菜单
来源：http://wng.jlsjyb.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vqk.cdnleiting.top

[R79] 解析命令行选项
来源：http://lpw.zhongyouzk.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zcb.yj20258.top

[R80] 查看脚本执行耗时
来源：http://ivp.jiagoushi.top

time ./run.sh
来源：http://kyk.uphjek.com

================================================================================
来源：http://woz.aizwys.cn

S. C / C++ 专题
来源：http://wls.bjfxy.top

================================================================================
来源：http://ijt.nanxuanxn.top

[S01] C：Hello World
来源：http://ovk.chenjidiqi.icu

#include <stdio.h>
来源：http://zdv.cucudq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://svr.daxiang520.top

[S02] C：变量与格式化输出
来源：http://dny.wangshuangyany.cn

int a = 10; printf("%d\n", a);
来源：http://udz.xylfe.cn

[S03] C：读入整数
来源：http://xwh.xingfuxueyuan.xyz

int x; scanf("%d", &x);
来源：http://okk.nwbrower.top

[S04] C：字符串复制
来源：http://yca.cheryme.top

char dst[32]; strcpy(dst, "hi");
来源：http://qzy.bbcook.cn

[S05] C：字符串长度
来源：http://uzh.jinghuilouyu.cn

strlen(s)
来源：http://pgd.zhixingplan.top

[S06] C：字符串比较
来源：http://lon.jinyuanbaomall.cn

strcmp(a, b) == 0
来源：http://xak.yj202588.top

[S07] C：数组遍历求和
来源：http://xhl.ivvv.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ghm.havefunace.top

[S08] C：动态内存分配与释放
来源：http://eme.fengsongda.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jlt.iojbl.cn

[S09] C：结构体定义与初始化
来源：http://tyn.daria6918.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iin.dashuyun.cn

[S10] C：指针与解引用
来源：http://rac.cdnleiting.top

int *p = &a;  *p = 5;
来源：http://lss.yfazqb.com

[S11] C：逐行读文件
来源：http://fjv.mhx1999.top

FILE *f = fopen("a.txt", "r");
来源：http://vcx.zhixingplan.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jht.jqgfzy.top

fclose(f);
来源：http://vfw.guowangkeji.top

[S12] C：写文件
来源：http://pvx.shanyushiyangtech.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zky.yanxiufei.cn

[S13] C：宏定义
来源：http://szl.shzxlz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://aqw.ehwqpu.com

[S14] C：枚举
来源：http://zdh.xinyue.icu

enum Color { RED, GREEN, BLUE };
来源：http://upz.smart0.xyz

[S15] C：类型转换
来源：http://gsv.yj20258.top

(double) a / b
来源：http://dii.zhixingplan.top

[S16] C：位操作置位
来源：http://uwq.c1oappe.top

x |= (1 << 3);
来源：http://usz.ivvv.top

[S17] C：安全拼接字符串
来源：http://mhw.52xcode.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hxr.hywenlv.cn

[S18] C：命令行参数
来源：http://mla.sxryk.cn

int main(int argc, char **argv)
来源：http://nzm.hammf.cn

[S19] C：快速排序
来源：http://ock.ydjk.org.cn

qsort(a, n, sizeof(int), cmp);
来源：http://atq.cashguo.top

[S20] C：二分查找
来源：http://qfx.pengpengdd.cyou

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mcr.hesvh.cn

[S21] C：字符类别判断
来源：http://iug.gaohongyu789.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://his.chenjidiqi.icu

[S22] C：字符串转数字
来源：http://tjf.guannengcc.top

atoi("42");  strtod("3.14", NULL);
来源：http://ybd.haohaochexian.top

[S23] C：随机数
来源：http://prl.ppjwa.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zev.yuanzhike.top

[S24] C：获取本地时间
来源：http://yuc.hywenlv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mgd.jianghu66.top

[S25] C：内存拷贝
来源：http://tlb.cqqwz.cn

memcpy(dst, src, n);
来源：http://clx.chenlongwang.top

[S26] C：内存清零
来源：http://hvd.gotoacloud.top

memset(a, 0, sizeof a);
来源：http://hxk.jqgufenzy.top

[S27] C：定义常量
来源：http://mav.jinqigfzy.top

const double PI = 3.14159;
来源：http://dtj.fanxiaobao.xyz

[S28] C：静态变量
来源：http://ddm.pengpengdd.cyou

static int counter = 0;
来源：http://pgs.tian-w.cn

[S29] C：变参函数
来源：http://pmc.zhijiandao.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vde.chenzaomai.com

[S30] C：头文件保护
来源：http://vsr.jqgfzy.top

#ifndef X_H
来源：http://uro.yuanzhike.top

#define X_H
来源：http://gcy.jinqigfzy.top

#endif
来源：http://ins.sxryk.cn

[S31] C++：Hello World
来源：http://qbk.daria6918.cn

#include <iostream>
来源：http://gau.hesvh.cn

int main() { std::cout << "Hello\n"; }
来源：http://eql.316326.xyz

[S32] C++：字符串
来源：http://fhr.yvedp.cn

std::string s = "hi";  s += "!";
来源：http://zla.shzxlz.cn

[S33] C++：vector 增删
来源：http://qgu.andypj.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nlt.yvedp.cn

[S34] C++：遍历 vector
来源：http://bud.zhaomingkeji.xyz

for (auto &x : v) { std::cout << x; }
来源：http://twd.birdmap.top

[S35] C++：map
来源：http://qto.jqgfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tjm.xinyue.icu

[S36] C++：unordered_map
来源：http://kvg.aizwys.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cdr.aizwys.cn

[S37] C++：set
来源：http://eov.kuanghao11.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jdk.xuetiantiany.cn

[S38] C++：排序
来源：http://grx.hnxiangtu.top

std::sort(v.begin(), v.end());
来源：http://sqc.ydjk.org.cn

[S39] C++：自定义比较器排序
来源：http://bfd.sysykeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dqk.chenlongwang.top

[S40] C++：查找元素
来源：http://jrf.zhixingplan.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xpi.fktsv.cn

[S41] C++：类与构造函数
来源：http://pje.daria6918.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lue.chenlongwang.top

[S42] C++：继承与虚函数
来源：http://czu.yanxiufei.cn

class B : public Base { public: void f() override {} };
来源：http://oml.ydzc1.top

[S43] C++：智能指针
来源：http://wrz.gzhubu.top

auto p = std::make_unique<int>(5);
来源：http://lve.hammf.cn

[S44] C++：引用传参
来源：http://efp.snrcjt.cn

void inc(int &x) { ++x; }
来源：http://nrl.xuetiantiany.cn

[S45] C++：lambda
来源：http://zay.feifeiyinyue.top

auto add = [](int a, int b) { return a + b; };
来源：http://cgh.yvedp.cn

[S46] C++：函数模板
来源：http://qbl.chenzaomai.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bwm.zhongyouzk.top

[S47] C++：结构化绑定遍历
来源：http://cin.shanyushiyangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vfg.jinghuilouyu.cn

[S48] C++：逐行读文件
来源：http://hdy.zdqjudy.top

std::ifstream in("a.txt");  std::string line;
来源：http://lfe.sufxvd.cn

while (std::getline(in, line)) { }
来源：http://ynd.hesvh.cn

[S49] C++：写文件
来源：http://now.shanyushiyangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hjk.tarul.cn

[S50] C++：格式化数字
来源：http://qfk.zhijiandao.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://asy.uphjek.com

[S51] C++：显式类型转换
来源：http://lge.nwbrower.top

static_cast<double>(a) / b
来源：http://myb.smart0.xyz

[S52] C++：const 与 noexcept
来源：http://jgw.epnwcf.com

int size() const noexcept { return n_; }
来源：http://dia.sxryk.cn

[S53] C++：移动语义
来源：http://kxs.yongpay.top

std::vector<int> w = std::move(v);
来源：http://jrd.sysykeji.top

[S54] C++：异常处理
来源：http://fwm.hnxiangtu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sdk.sxryk.cn

[S55] C++：结构化绑定
来源：http://lyu.yuanzhike.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pod.shuidangran.top

[S56] C++：optional
来源：http://owo.wangdashe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yis.yueranfly.top

[S57] C++：编译期常量
来源：http://ibg.hnxiangtu.top

constexpr int N = 10;
来源：http://pyr.chenjidiqi.icu

[S58] C++：命名空间
来源：http://oyp.snrcjt.cn

namespace ns { int f() { return 1; } }
来源：http://bxa.sufxvd.cn

[S59] C++：静态断言
来源：http://zcv.smart0.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cdj.nanxuanxn.top

[S60] C++：遍历并删除元素
来源：http://mbk.smart0.xyz


<!-- 参考信息 -->