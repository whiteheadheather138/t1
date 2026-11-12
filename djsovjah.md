代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://grf.yj202588.top

[Q90] 生成序号列
来源：http://htg.zhixingplan.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mpr.jqgufenzy.top

================================================================================
来源：http://ygu.zhixingplan.top

R. Bash 专题
来源：http://dhv.jianghu66.top

================================================================================
来源：http://wws.birdmap.top

[R01] shebang 与严格模式
来源：http://uai.vehdjk.com

#!/usr/bin/env bash
来源：http://vzw.hfpthk.cn

set -euo pipefail
来源：http://vgx.hammf.cn

[R02] 变量赋值与使用
来源：http://kve.ppjwa.cn

name="Tom"; echo "$name"
来源：http://eap.pengpengdd.cyou

[R03] 只读变量
来源：http://vnp.tanke756.top

readonly PI=3.14
来源：http://pom.svipenyu.cn

[R04] 位置参数
来源：http://fkb.pycfn.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://smj.hcnkem.com

[R05] 参数默认值
来源：http://wup.xingfuxueyuan.xyz

name="${1:-default}"
来源：http://qzd.zhiwuduotai.top

[R06] 判断命令是否存在
来源：http://qhu.xingfuxueyuan.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://muo.nwbrower.top

[R07] if 判断文件
来源：http://mlb.yongpay.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bsf.ppjwa.cn

[R08] 数值比较
来源：http://dlo.wangshuangyany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://chn.zhongyouzk.top

[R09] 字符串比较
来源：http://dra.dianchejie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jgc.jyoumei.cn

[R10] 正则匹配
来源：http://fkc.yongpay.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hlh.wangdashe.top

[R11] case 多分支
来源：http://civ.jinqigufen.top

case "$1" in
来源：http://bik.shanyushiyangkeji.top

start) echo "启动" ;;
来源：http://auw.hysaishi.cn

stop)  echo "停止" ;;
来源：http://qgw.vehdjk.com

*)     echo "未知命令" ;;
来源：http://azy.hnqzz.top

esac
来源：http://wel.hfpthk.cn

[R12] for 遍历文件
来源：http://qsr.kuanghao11.cn

for f in *.txt; do echo "$f"; done
来源：http://sgh.quarkkingdee.top

[R13] for 计数循环
来源：http://whe.c1oappe.top

for i in {1..10}; do echo "$i"; done
来源：http://rvc.ivvv.top

[R14] C 风格 for
来源：http://sjt.havefunace.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dti.xylfe.cn

[R15] while 逐行读文件
来源：http://iua.iojbl.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gmj.feifeiyinyue.top

[R16] until 等待条件
来源：http://eic.jiagoushi.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rym.kuanghao11.cn

[R17] 数组定义与取值
来源：http://fvz.meibo888.top

arr=(a b c); echo "${arr[0]}"
来源：http://qep.yonumen.top

[R18] 遍历数组
来源：http://mri.cucudq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rie.cdnleiting.top

[R19] 数组长度
来源：http://oup.tanke756.top

echo "${#arr[@]}"
来源：http://fsp.chenjidiqi.icu

[R20] 关联数组（字典）
来源：http://ine.jianghu66.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lit.daxiang520.top

[R21] 字符串长度
来源：http://ymv.0kj1m.cn

echo "${#s}"
来源：http://qlq.quarkkingdee.top

[R22] 截取子串
来源：http://cmt.sweek.top

echo "${s:0:5}"
来源：http://nta.zhijiandao.cn

[R23] 字符串替换
来源：http://oot.pycfn.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ugs.shangyingyoupin.top

[R24] 大小写转换
来源：http://gei.fengsongda.top

echo "${s^^}"; echo "${s,,}"
来源：http://oqj.bbcook.cn

[R25] 去后缀 / 去前缀
来源：http://vhd.ppjwa.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qom.zhixingplan.top

[R26] 命令替换
来源：http://sui.shanyushiyangkeji.top

now=$(date +%F); echo "$now"
来源：http://zvm.yj20258888.top

[R27] 算术展开
来源：http://qvc.0kj1m.cn

echo $((1 + 2 * 3))
来源：http://mmq.ywan-chungtsiang.top

[R28] 浮点运算
来源：http://wya.fktsv.cn

echo "scale=2; 10/3" | bc
来源：http://lqr.hesvh.cn

[R29] 定义函数
来源：http://qaz.smart0.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://txv.yvedp.cn

[R30] 函数返回状态码
来源：http://rnr.jianghu66.top

f() { return 0; }; f || echo "失败了"
来源：http://ywo.zhoulong.xyz

[R31] 局部变量
来源：http://nvz.hywenlv.cn

f() { local x=1; echo "$x"; }
来源：http://jmz.aizwys.cn

[R32] 参数个数校验
来源：http://mar.52xcode.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eap.tanke756.top

[R33] 捕获错误并提示行号
来源：http://aej.jinghuilouyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nxr.xuanzx.com

[R34] 退出时清理
来源：http://psd.dianchejie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yat.zhixingplan.top

[R35] 后台执行并等待
来源：http://pyl.chenlongwang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wxn.chenjidiqi.icu

[R36] 并发执行多个任务
来源：http://rqh.sjlbkw.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jdl.sweek.top

[R37] 把输出赋给变量
来源：http://ude.epnwcf.com

files=$(ls -1)
来源：http://rmw.pycfn.com

[R38] 管道串联
来源：http://ksq.jlsjyb.cn

cat a.txt | grep -i error | wc -l
来源：http://hwo.sjlbkw.cn

[R39] 重定向标准输出与错误
来源：http://nvl.jqgfzy.top

cmd > out.log 2>&1
来源：http://xxi.vqdsnc.cn

[R40] 追加写日志
来源：http://ffb.snrcjt.cn

echo "log" >> out.log
来源：http://hik.cheryme.top

[R41] 丢弃输出
来源：http://tio.aizwys.cn

cmd >/dev/null 2>&1
来源：http://reu.hywenlv.cn

[R42] 输入重定向
来源：http://cad.dashuyun.cn

wc -l < a.txt
来源：http://psl.svipenyu.cn

[R43] 按名字查找文件
来源：http://mss.fktsv.cn

find . -name "*.log" -type f
来源：http://sjr.meibo888.top

[R44] 按修改时间查找
来源：http://qsd.gogol.net.cn

find . -mtime -7 -type f
来源：http://dci.sxryk.cn

[R45] 批量删除
来源：http://snu.chenjidiqi.icu

find . -name "*.tmp" -delete
来源：http://toz.redwolf501.top

[R46] 递归替换文件内容
来源：http://ygn.shanyushiyangtech.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mej.nanxinkj.top

[R47] sed 单行替换
来源：http://mfo.nanxuanxn.top

sed -i 's/foo/bar/g' a.txt
来源：http://xjq.xinyue.icu

[R48] awk 取指定列
来源：http://hse.jyoumei.cn

awk '{print $1, $3}' a.txt
来源：http://tzj.iojbl.cn

[R49] awk 带条件
来源：http://yba.chenzaomai.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://flg.ybcxt.top

[R50] awk 求和
来源：http://obf.wangshuangyany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wnk.jinqigfzy.top

[R51] 排序去重取前几
来源：http://ynq.wangshuangyany.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kgp.yfazqb.com

[R52] 统计行数
来源：http://ush.fzhhl.top

wc -l a.txt
来源：http://rmj.ybcxt.top

[R53] 查看文件头与实时尾
来源：http://ylp.feifeiyinyue.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rld.fzhhl.top

[R54] 比较两个文件
来源：http://nqj.wangdashe.top

diff a.txt b.txt
来源：http://qcb.chenlongwang.top

[R55] 压缩与解压
来源：http://rfq.316326.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lzj.gaohongyu789.top

[R56] 远程拷贝
来源：http://kem.andypj.xyz

scp file user@host:/path/
来源：http://mwp.hcnkem.com

[R57] 远程执行命令
来源：http://lam.xuetiantiany.cn

ssh user@host 'uptime'
来源：http://bwv.zhixingplan.top

[R58] 下载文件
来源：http://tod.pengpengdd.cyou

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ecv.zdqjudy.top

[R59] 发 POST JSON
来源：http://ttf.hongshengwenyu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fnu.ydjk.org.cn

[R60] 只看 HTTP 状态码
来源：http://mys.yanxiufei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hxo.nanxinkj.top

[R61] 磁盘占用
来源：http://jvm.hnqzz.top

df -h;  du -sh *
来源：http://ssg.cheryme.top

[R62] 找最占空间的文件
来源：http://tbv.ivvv.top

du -ah . | sort -rh | head -10
来源：http://kbk.316326.xyz

[R63] 内存与进程
来源：http://mgx.nanxuanxn.top

free -h;  ps aux | grep nginx
来源：http://uva.tian-w.cn

[R64] 结束进程
来源：http://uqr.chenlongwang.top

kill -9 $(pgrep -f app.py)
来源：http://lsj.xuanzx.com

[R65] 查看端口占用
来源：http://kgm.iojbl.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vhv.ehwqpu.com

[R66] 定时任务
来源：http://jsc.hcnkem.com

crontab -e;  crontab -l
来源：http://bpw.zdbjq.cn

[R67] 生成随机十六进制串
来源：http://wgr.hcnkem.com

openssl rand -hex 16
来源：http://mgn.chenzaomai.com

[R68] 计算文件校验值
来源：http://gwn.sufxvd.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dfv.fehbvm.com

[R69] 生成随机密码
来源：http://ert.yvedp.cn

head -c 16 /dev/urandom | base64
来源：http://hyw.daria6918.cn

[R70] 时间戳与互转
来源：http://qif.jqgufenzy.top

date +%s;  date -d @1700000000
来源：http://rns.dashuyun.cn

[R71] 日期格式化
来源：http://zbx.daxiang520.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jlr.yueranfly.top

[R72] 等待端口就绪
来源：http://sgw.yanxiufei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://evl.tianlin.xyz

[R73] 分割大日志
来源：http://lvg.quarkkingdee.top

split -l 1000 big.log part_
来源：http://jbh.316326.xyz

[R74] 批量重命名
来源：http://zvi.vqdsnc.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://agr.tanke756.top

[R75] 导出环境变量
来源：http://iad.sxryk.cn

export PATH="$HOME/bin:$PATH"
来源：http://qzc.hfpthk.cn

[R76] 使用临时文件
来源：http://kqu.ehwqpu.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rlh.andypj.xyz

[R77] 读取用户输入
来源：http://fje.sysykeji.top

read -rp "请输入: " ans
来源：http://xuf.jqgufenzy.top

[R78] 交互式菜单
来源：http://xju.zhijiandao.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wsy.sweek.top

[R79] 解析命令行选项
来源：http://fao.nanxuanxn.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sef.ywan-chungtsiang.top

[R80] 查看脚本执行耗时
来源：http://hfh.meibo888.top

time ./run.sh
来源：http://fon.wangshuangyany.cn

================================================================================
来源：http://guv.yuanzhike.top

S. C / C++ 专题
来源：http://skl.zdqjudy.top

================================================================================
来源：http://knk.jqgufenzy.top

[S01] C：Hello World
来源：http://koc.redwolf501.top

#include <stdio.h>
来源：http://neh.9152youxi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bmq.iojbl.cn

[S02] C：变量与格式化输出
来源：http://yxb.havefunace.top

int a = 10; printf("%d\n", a);
来源：http://ntp.jinyuanbaomall.cn

[S03] C：读入整数
来源：http://rap.ybcxt.top

int x; scanf("%d", &x);
来源：http://xal.yongpay.top

[S04] C：字符串复制
来源：http://yzf.sjlbkw.cn

char dst[32]; strcpy(dst, "hi");
来源：http://eaj.xingfuxueyuan.xyz

[S05] C：字符串长度
来源：http://gkj.xingfuxueyuan.xyz

strlen(s)
来源：http://oda.yangfankeji.com

[S06] C：字符串比较
来源：http://rlw.jinqigfzy.top

strcmp(a, b) == 0
来源：http://wgq.sysykeji.top

[S07] C：数组遍历求和
来源：http://ibq.zdbjq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rqk.ydzc1.top

[S08] C：动态内存分配与释放
来源：http://zpz.sufxvd.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gpf.tarul.cn

[S09] C：结构体定义与初始化
来源：http://ljy.cdnleiting.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://igx.xylfe.cn

[S10] C：指针与解引用
来源：http://pix.cashguo.top

int *p = &a;  *p = 5;
来源：http://erq.jinghuilouyu.cn

[S11] C：逐行读文件
来源：http://mmf.zycfv.cn

FILE *f = fopen("a.txt", "r");
来源：http://txt.iojbl.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fli.cashguo.top

fclose(f);
来源：http://xea.xziqi.cn

[S12] C：写文件
来源：http://nje.pengpengdd.cyou

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fmh.shzxlz.cn

[S13] C：宏定义
来源：http://rdv.jlsjyb.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uvh.hywenlv.cn

[S14] C：枚举
来源：http://vhf.tanke756.top

enum Color { RED, GREEN, BLUE };
来源：http://dyc.zycfv.cn

[S15] C：类型转换
来源：http://rhw.redwolf501.top

(double) a / b
来源：http://mlq.vehdjk.com

[S16] C：位操作置位
来源：http://atv.fehbvm.com

x |= (1 << 3);
来源：http://rik.hywenlv.cn

[S17] C：安全拼接字符串
来源：http://kmv.jianghu66.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wyu.c1oappe.top

[S18] C：命令行参数
来源：http://bgy.redwolf501.top

int main(int argc, char **argv)
来源：http://cok.wangshuangyany.cn

[S19] C：快速排序
来源：http://kpw.ppjwa.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kpc.hysaishi.cn

[S20] C：二分查找
来源：http://qdb.hongshengwenyu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ieq.jqgfzy.top

[S21] C：字符类别判断
来源：http://kla.andypj.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cce.uphjek.com

[S22] C：字符串转数字
来源：http://lpf.smart0.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://urw.yongpay.top

[S23] C：随机数
来源：http://kdr.yj20258.top

srand(time(NULL));  int r = rand() % 100;
来源：http://thd.yanxiufei.cn

[S24] C：获取本地时间
来源：http://itf.c1oappe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xkb.shzxlz.cn

[S25] C：内存拷贝
来源：http://mku.gogol.net.cn

memcpy(dst, src, n);
来源：http://knw.52xcode.cn

[S26] C：内存清零
来源：http://kkz.havefunace.top

memset(a, 0, sizeof a);
来源：http://dpl.zhiwuduotai.top

[S27] C：定义常量
来源：http://vvi.hfpthk.cn

const double PI = 3.14159;
来源：http://crk.meibo888.top

[S28] C：静态变量
来源：http://zpv.ydjk.org.cn

static int counter = 0;
来源：http://ucc.cucudq.cn

[S29] C：变参函数
来源：http://vki.316326.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://leu.sweek.top

[S30] C：头文件保护
来源：http://mge.feifeiyinyue.top

#ifndef X_H
来源：http://oan.jinqigfzy.top

#define X_H
来源：http://mob.chenlongwang.top

#endif
来源：http://fmm.shangyingyoupin.top

[S31] C++：Hello World
来源：http://eyd.shangyingyoupin.top

#include <iostream>
来源：http://ixn.aibaodan.cn

int main() { std::cout << "Hello\n"; }
来源：http://mab.tarul.cn

[S32] C++：字符串
来源：http://dpv.xuetiantiany.cn

std::string s = "hi";  s += "!";
来源：http://box.yonumen.top

[S33] C++：vector 增删
来源：http://nvr.chenzaomai.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pia.zhoulong.xyz

[S34] C++：遍历 vector
来源：http://eut.bbcook.cn

for (auto &x : v) { std::cout << x; }
来源：http://ffy.shuidangran.top

[S35] C++：map
来源：http://sjn.sxryk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ava.quarkkingdee.top

[S36] C++：unordered_map
来源：http://bib.pycfn.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vgc.yueranfly.top

[S37] C++：set
来源：http://pmi.cheryme.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rst.yvedp.cn

[S38] C++：排序
来源：http://urk.zhaomingkeji.xyz

std::sort(v.begin(), v.end());
来源：http://hvt.feifeiyinyue.top

[S39] C++：自定义比较器排序
来源：http://cjw.zhoulong.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kaa.uphjek.com

[S40] C++：查找元素
来源：http://hzd.svipenyu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://esa.jqgufenzy.top

[S41] C++：类与构造函数
来源：http://jvo.yuanzhike.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uuf.tian-w.cn

[S42] C++：继承与虚函数
来源：http://ztt.cheryme.top

class B : public Base { public: void f() override {} };
来源：http://bgw.gzhubu.top

[S43] C++：智能指针
来源：http://smg.yanxiufei.cn

auto p = std::make_unique<int>(5);
来源：http://oll.xingfuxueyuan.xyz

[S44] C++：引用传参
来源：http://cmp.jqgfzy.top

void inc(int &x) { ++x; }
来源：http://oht.vehdjk.com

[S45] C++：lambda
来源：http://ezd.smart0.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://ppn.52xcode.cn

[S46] C++：函数模板
来源：http://frh.sufxvd.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bvy.jiagoushi.top

[S47] C++：结构化绑定遍历
来源：http://ced.hnxiangtu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yaz.yvedp.cn

[S48] C++：逐行读文件
来源：http://sjn.xuanzx.com

std::ifstream in("a.txt");  std::string line;
来源：http://hxc.yanxiufei.cn

while (std::getline(in, line)) { }
来源：http://cgb.ivvv.top

[S49] C++：写文件
来源：http://ndc.fktsv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dgs.snrcjt.cn

[S50] C++：格式化数字
来源：http://frp.xylfe.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fsd.jinqigufen.top

[S51] C++：显式类型转换
来源：http://njr.havefunace.top

static_cast<double>(a) / b
来源：http://chi.tanke756.top

[S52] C++：const 与 noexcept
来源：http://uui.fanxiaobao.xyz

int size() const noexcept { return n_; }
来源：http://laq.cheryme.top

[S53] C++：移动语义
来源：http://rol.uphjek.com

std::vector<int> w = std::move(v);
来源：http://lht.gaohongyu789.top

[S54] C++：异常处理
来源：http://xfv.guannengcc.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xpu.andypj.xyz

[S55] C++：结构化绑定
来源：http://kks.wangshuangyany.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sxi.chenzaomai.com

[S56] C++：optional
来源：http://yro.cucudq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://grb.pycfn.com

[S57] C++：编译期常量
来源：http://wup.yj20258.top

constexpr int N = 10;
来源：http://son.jlsjyb.cn

[S58] C++：命名空间
来源：http://qbg.c1oappe.top

namespace ns { int f() { return 1; } }
来源：http://iar.zhoulong.xyz

[S59] C++：静态断言
来源：http://poj.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mvo.kuanghao11.cn

[S60] C++：遍历并删除元素
来源：http://gnt.cdnleiting.top


<!-- 参考信息 -->