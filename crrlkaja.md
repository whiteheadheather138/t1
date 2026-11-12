代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://voa.andypj.xyz

[Q90] 生成序号列
来源：http://dyn.chenjidiqi.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vfs.guannengcc.top

================================================================================
来源：http://coe.kuanghao11.cn

R. Bash 专题
来源：http://bfk.gotoacloud.top

================================================================================
来源：http://egr.yuxming.cn

[R01] shebang 与严格模式
来源：http://fjb.fehbvm.com

#!/usr/bin/env bash
来源：http://ipp.nwbrower.top

set -euo pipefail
来源：http://afs.guannengcc.top

[R02] 变量赋值与使用
来源：http://liz.sweek.top

name="Tom"; echo "$name"
来源：http://wwq.c1oappe.top

[R03] 只读变量
来源：http://jfx.dianchejie.cn

readonly PI=3.14
来源：http://ccu.nanxinkj.top

[R04] 位置参数
来源：http://gyc.xuanzx.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gao.fzhhl.top

[R05] 参数默认值
来源：http://arx.cucudq.cn

name="${1:-default}"
来源：http://yth.zycfv.cn

[R06] 判断命令是否存在
来源：http://dxf.hongshengwenyu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pjk.yuanzhike.top

[R07] if 判断文件
来源：http://kcy.xziqi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ipk.zdqjudy.top

[R08] 数值比较
来源：http://mrb.ywan-chungtsiang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://gfd.vqdsnc.cn

[R09] 字符串比较
来源：http://bcl.xinyue.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wbe.ywan-chungtsiang.top

[R10] 正则匹配
来源：http://aop.0kj1m.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jxs.bbcook.cn

[R11] case 多分支
来源：http://ldo.snrcjt.cn

case "$1" in
来源：http://glm.xuanzx.com

start) echo "启动" ;;
来源：http://bmo.redwolf501.top

stop)  echo "停止" ;;
来源：http://icc.c1oappe.top

*)     echo "未知命令" ;;
来源：http://oow.yongpay.top

esac
来源：http://nvd.uphjek.com

[R12] for 遍历文件
来源：http://akw.zhongyouzk.top

for f in *.txt; do echo "$f"; done
来源：http://wlt.andypj.xyz

[R13] for 计数循环
来源：http://isr.ppjwa.cn

for i in {1..10}; do echo "$i"; done
来源：http://leh.aibaodan.cn

[R14] C 风格 for
来源：http://bic.guannengcc.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hxy.sweek.top

[R15] while 逐行读文件
来源：http://khq.svipenyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fwr.yj20258888.top

[R16] until 等待条件
来源：http://efm.ehwqpu.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://egf.birdmap.top

[R17] 数组定义与取值
来源：http://wop.ydzc1.top

arr=(a b c); echo "${arr[0]}"
来源：http://ygu.zdqjudy.top

[R18] 遍历数组
来源：http://fqo.yuxming.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fzd.ywan-chungtsiang.top

[R19] 数组长度
来源：http://vnq.hammf.cn

echo "${#arr[@]}"
来源：http://cyz.tanke756.top

[R20] 关联数组（字典）
来源：http://hxf.sysykeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rep.jyoumei.cn

[R21] 字符串长度
来源：http://xeg.daria6918.cn

echo "${#s}"
来源：http://dbe.jinqigfzy.top

[R22] 截取子串
来源：http://zvi.nanxuanxn.top

echo "${s:0:5}"
来源：http://ttd.tianlin.xyz

[R23] 字符串替换
来源：http://znn.zhijiandao.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xqp.jiagoushi.top

[R24] 大小写转换
来源：http://ocp.chenlongwang.top

echo "${s^^}"; echo "${s,,}"
来源：http://ovy.ehwqpu.com

[R25] 去后缀 / 去前缀
来源：http://izh.mhx1999.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://cgv.ywan-chungtsiang.top

[R26] 命令替换
来源：http://aiz.yueranfly.top

now=$(date +%F); echo "$now"
来源：http://xck.uphjek.com

[R27] 算术展开
来源：http://qya.wangshuangyany.cn

echo $((1 + 2 * 3))
来源：http://nez.redwolf501.top

[R28] 浮点运算
来源：http://hpe.sysykeji.top

echo "scale=2; 10/3" | bc
来源：http://uma.nanxinkj.top

[R29] 定义函数
来源：http://mle.shanyushiyangtech.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tnm.hnqzz.top

[R30] 函数返回状态码
来源：http://lpe.birdmap.top

f() { return 0; }; f || echo "失败了"
来源：http://son.316326.xyz

[R31] 局部变量
来源：http://bog.fzhhl.top

f() { local x=1; echo "$x"; }
来源：http://mbx.vqdsnc.cn

[R32] 参数个数校验
来源：http://yvi.gaohongyu789.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cro.cashguo.top

[R33] 捕获错误并提示行号
来源：http://gnf.shanyushiyangtech.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tri.jianghu66.top

[R34] 退出时清理
来源：http://ntv.yj202588.top

trap 'rm -f "$tmp"' EXIT
来源：http://nik.yj20258.top

[R35] 后台执行并等待
来源：http://epo.kuanghao11.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yls.0kj1m.cn

[R36] 并发执行多个任务
来源：http://zlq.kuanghao11.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bfl.snrcjt.cn

[R37] 把输出赋给变量
来源：http://jiw.birdmap.top

files=$(ls -1)
来源：http://hqq.andypj.xyz

[R38] 管道串联
来源：http://lvc.jyoumei.cn

cat a.txt | grep -i error | wc -l
来源：http://jlz.andypj.xyz

[R39] 重定向标准输出与错误
来源：http://ibd.gogol.net.cn

cmd > out.log 2>&1
来源：http://ygi.xinyue.icu

[R40] 追加写日志
来源：http://ldm.uphjek.com

echo "log" >> out.log
来源：http://crg.wangdashe.top

[R41] 丢弃输出
来源：http://epo.chenjidiqi.icu

cmd >/dev/null 2>&1
来源：http://lvc.fehbvm.com

[R42] 输入重定向
来源：http://yeq.xingfuxueyuan.xyz

wc -l < a.txt
来源：http://izh.316326.xyz

[R43] 按名字查找文件
来源：http://drk.pengpengdd.cyou

find . -name "*.log" -type f
来源：http://mtw.316326.xyz

[R44] 按修改时间查找
来源：http://fhk.uphjek.com

find . -mtime -7 -type f
来源：http://iiw.hnxiangtu.top

[R45] 批量删除
来源：http://ldl.shanyushiyangkeji.top

find . -name "*.tmp" -delete
来源：http://tgm.gzhubu.top

[R46] 递归替换文件内容
来源：http://fxx.vehdjk.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gmx.jinghuilouyu.cn

[R47] sed 单行替换
来源：http://plm.havefunace.top

sed -i 's/foo/bar/g' a.txt
来源：http://tur.xylfe.cn

[R48] awk 取指定列
来源：http://mxv.feifeiyinyue.top

awk '{print $1, $3}' a.txt
来源：http://gkh.ybcxt.top

[R49] awk 带条件
来源：http://mxn.hammf.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://roc.tarul.cn

[R50] awk 求和
来源：http://ktw.xuetiantiany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://frz.vqdsnc.cn

[R51] 排序去重取前几
来源：http://zfe.yuanzhike.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ait.jlsjyb.cn

[R52] 统计行数
来源：http://wep.hcnkem.com

wc -l a.txt
来源：http://kcg.dianchejie.cn

[R53] 查看文件头与实时尾
来源：http://rjs.cashguo.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ndx.gotoacloud.top

[R54] 比较两个文件
来源：http://akx.yj202588.top

diff a.txt b.txt
来源：http://fhv.jinqigufen.top

[R55] 压缩与解压
来源：http://vxa.gaohongyu789.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://exv.nanxinkj.top

[R56] 远程拷贝
来源：http://erg.chenlongwang.top

scp file user@host:/path/
来源：http://bsp.fengsongda.top

[R57] 远程执行命令
来源：http://qpy.fengsongda.top

ssh user@host 'uptime'
来源：http://tsb.jqgfzy.top

[R58] 下载文件
来源：http://pqh.cashguo.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ksl.zhoulong.xyz

[R59] 发 POST JSON
来源：http://esl.hesvh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://api.zhoulong.xyz

[R60] 只看 HTTP 状态码
来源：http://lrw.yuxming.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ulw.yueranfly.top

[R61] 磁盘占用
来源：http://uxn.meibo888.top

df -h;  du -sh *
来源：http://tqv.yfazqb.com

[R62] 找最占空间的文件
来源：http://lat.guannengcc.top

du -ah . | sort -rh | head -10
来源：http://grb.shangyingyoupin.top

[R63] 内存与进程
来源：http://ndy.yongpay.top

free -h;  ps aux | grep nginx
来源：http://rwv.nwbrower.top

[R64] 结束进程
来源：http://upr.yvedp.cn

kill -9 $(pgrep -f app.py)
来源：http://gmr.kuanghao11.cn

[R65] 查看端口占用
来源：http://nou.jianghu66.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://iew.sjlbkw.cn

[R66] 定时任务
来源：http://uln.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://fdv.daxiang520.top

[R67] 生成随机十六进制串
来源：http://dsg.chenjidiqi.icu

openssl rand -hex 16
来源：http://qjs.0kj1m.cn

[R68] 计算文件校验值
来源：http://ejl.gzhubu.top

sha256sum a.txt;  md5sum a.txt
来源：http://wej.shanyushiyangkeji.top

[R69] 生成随机密码
来源：http://hog.zhoulong.xyz

head -c 16 /dev/urandom | base64
来源：http://fim.sweek.top

[R70] 时间戳与互转
来源：http://wri.fktsv.cn

date +%s;  date -d @1700000000
来源：http://egj.tanke756.top

[R71] 日期格式化
来源：http://xcr.tian-w.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qrn.yanxiufei.cn

[R72] 等待端口就绪
来源：http://dcy.yueranfly.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dal.shuidangran.top

[R73] 分割大日志
来源：http://zni.jianghu66.top

split -l 1000 big.log part_
来源：http://tdy.ywan-chungtsiang.top

[R74] 批量重命名
来源：http://ipa.zhoulong.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://puc.316326.xyz

[R75] 导出环境变量
来源：http://jtx.snrcjt.cn

export PATH="$HOME/bin:$PATH"
来源：http://nkr.cashguo.top

[R76] 使用临时文件
来源：http://caq.vehdjk.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ftz.zycfv.cn

[R77] 读取用户输入
来源：http://dkp.vqdsnc.cn

read -rp "请输入: " ans
来源：http://dgt.dashuyun.cn

[R78] 交互式菜单
来源：http://cpo.gaohongyu789.top

select opt in a b c; do echo "$opt"; break; done
来源：http://elf.jqgufenzy.top

[R79] 解析命令行选项
来源：http://zvn.yuxming.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sgj.hysaishi.cn

[R80] 查看脚本执行耗时
来源：http://uct.zhiwuduotai.top

time ./run.sh
来源：http://uak.cucudq.cn

================================================================================
来源：http://adu.hesvh.cn

S. C / C++ 专题
来源：http://hmw.shanyushiyangkeji.top

================================================================================
来源：http://nvq.hesvh.cn

[S01] C：Hello World
来源：http://wgt.xuanzx.com

#include <stdio.h>
来源：http://tcs.tanke756.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ean.smart0.xyz

[S02] C：变量与格式化输出
来源：http://qzn.smart0.xyz

int a = 10; printf("%d\n", a);
来源：http://tfw.sysykeji.top

[S03] C：读入整数
来源：http://mcx.gogol.net.cn

int x; scanf("%d", &x);
来源：http://rcl.hnqzz.top

[S04] C：字符串复制
来源：http://zsb.jqgfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://bxv.zdqjudy.top

[S05] C：字符串长度
来源：http://dfb.jinqigfzy.top

strlen(s)
来源：http://fxl.zhongyouzk.top

[S06] C：字符串比较
来源：http://mhj.dashuyun.cn

strcmp(a, b) == 0
来源：http://lnx.jianghu66.top

[S07] C：数组遍历求和
来源：http://nej.yangfankeji.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://spj.gotoacloud.top

[S08] C：动态内存分配与释放
来源：http://wzr.chenlongwang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zwv.shanyushiyangkeji.top

[S09] C：结构体定义与初始化
来源：http://uhu.daxiang520.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://acc.zhengqikj.top

[S10] C：指针与解引用
来源：http://jop.hcnkem.com

int *p = &a;  *p = 5;
来源：http://ryr.jqgfzy.top

[S11] C：逐行读文件
来源：http://jce.zhongyouzk.top

FILE *f = fopen("a.txt", "r");
来源：http://cwo.haohaochexian.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://glr.hysaishi.cn

fclose(f);
来源：http://ojv.hcnkem.com

[S12] C：写文件
来源：http://axe.jinqigfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qzc.hywenlv.cn

[S13] C：宏定义
来源：http://oww.shzxlz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uza.fengsongda.top

[S14] C：枚举
来源：http://alo.hcnkem.com

enum Color { RED, GREEN, BLUE };
来源：http://jgg.tarul.cn

[S15] C：类型转换
来源：http://kuz.sufxvd.cn

(double) a / b
来源：http://tnf.cheryme.top

[S16] C：位操作置位
来源：http://tau.cqqwz.cn

x |= (1 << 3);
来源：http://suk.yangfankeji.com

[S17] C：安全拼接字符串
来源：http://mxt.ybcxt.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hpi.yueranfly.top

[S18] C：命令行参数
来源：http://ehy.xingfuxueyuan.xyz

int main(int argc, char **argv)
来源：http://sum.sufxvd.cn

[S19] C：快速排序
来源：http://hlr.ctjpmb.com

qsort(a, n, sizeof(int), cmp);
来源：http://qlf.jqgufenzy.top

[S20] C：二分查找
来源：http://wlc.iojbl.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cfl.yonumen.top

[S21] C：字符类别判断
来源：http://pzn.yj202588.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://big.shanyushiyangkeji.top

[S22] C：字符串转数字
来源：http://fif.yanxiufei.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dfh.316326.xyz

[S23] C：随机数
来源：http://coj.sjlbkw.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jld.xuetiantiany.cn

[S24] C：获取本地时间
来源：http://onc.haohaochexian.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mkk.jinqigufen.top

[S25] C：内存拷贝
来源：http://rtw.xziqi.cn

memcpy(dst, src, n);
来源：http://rxz.jlsjyb.cn

[S26] C：内存清零
来源：http://poy.ywan-chungtsiang.top

memset(a, 0, sizeof a);
来源：http://wit.gotoacloud.top

[S27] C：定义常量
来源：http://ypc.sufxvd.cn

const double PI = 3.14159;
来源：http://gop.shzxlz.cn

[S28] C：静态变量
来源：http://iva.shangyingyoupin.top

static int counter = 0;
来源：http://jod.shanyushiyangkeji.top

[S29] C：变参函数
来源：http://cgv.cashguo.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dmc.cheryme.top

[S30] C：头文件保护
来源：http://bjf.daxiang520.top

#ifndef X_H
来源：http://xgz.ivvv.top

#define X_H
来源：http://kmf.yj20258888.top

#endif
来源：http://gpz.daxiang520.top

[S31] C++：Hello World
来源：http://ysc.hysaishi.cn

#include <iostream>
来源：http://bda.fehbvm.com

int main() { std::cout << "Hello\n"; }
来源：http://bpt.jinqigufen.top

[S32] C++：字符串
来源：http://edl.yonumen.top

std::string s = "hi";  s += "!";
来源：http://iti.cdnleiting.top

[S33] C++：vector 增删
来源：http://fbl.ehwqpu.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hrj.zycfv.cn

[S34] C++：遍历 vector
来源：http://agu.jlsjyb.cn

for (auto &x : v) { std::cout << x; }
来源：http://hrw.hammf.cn

[S35] C++：map
来源：http://zsu.nanxuanxn.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tuc.zhiwuduotai.top

[S36] C++：unordered_map
来源：http://fwh.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ize.jianghu66.top

[S37] C++：set
来源：http://guu.yvedp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ott.uphjek.com

[S38] C++：排序
来源：http://dxk.tianlin.xyz

std::sort(v.begin(), v.end());
来源：http://fin.nanxuanxn.top

[S39] C++：自定义比较器排序
来源：http://gwz.shangyingyoupin.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wih.52xcode.cn

[S40] C++：查找元素
来源：http://idj.tanke756.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hjy.shuidangran.top

[S41] C++：类与构造函数
来源：http://xfa.hesvh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dsw.smart0.xyz

[S42] C++：继承与虚函数
来源：http://gok.xinyue.icu

class B : public Base { public: void f() override {} };
来源：http://ygh.dashuyun.cn

[S43] C++：智能指针
来源：http://uxg.nanxinkj.top

auto p = std::make_unique<int>(5);
来源：http://tro.iojbl.cn

[S44] C++：引用传参
来源：http://llw.sweek.top

void inc(int &x) { ++x; }
来源：http://sgd.chenzaomai.com

[S45] C++：lambda
来源：http://bct.chenlongwang.top

auto add = [](int a, int b) { return a + b; };
来源：http://kum.uphjek.com

[S46] C++：函数模板
来源：http://lws.hammf.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gvw.cqqwz.cn

[S47] C++：结构化绑定遍历
来源：http://nbc.xziqi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ytv.0kj1m.cn

[S48] C++：逐行读文件
来源：http://sus.gaohongyu789.top

std::ifstream in("a.txt");  std::string line;
来源：http://agf.xziqi.cn

while (std::getline(in, line)) { }
来源：http://cct.shangyingyoupin.top

[S49] C++：写文件
来源：http://zvw.fengsongda.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mxz.zhiwuduotai.top

[S50] C++：格式化数字
来源：http://pzb.vehdjk.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uld.dashuyun.cn

[S51] C++：显式类型转换
来源：http://imq.yj20258888.top

static_cast<double>(a) / b
来源：http://ezu.hammf.cn

[S52] C++：const 与 noexcept
来源：http://voy.cqqwz.cn

int size() const noexcept { return n_; }
来源：http://zbg.fzhhl.top

[S53] C++：移动语义
来源：http://ddg.fanxiaobao.xyz

std::vector<int> w = std::move(v);
来源：http://iog.chenjidiqi.icu

[S54] C++：异常处理
来源：http://xzc.kuanghao11.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xtv.hcnkem.com

[S55] C++：结构化绑定
来源：http://kqt.0kj1m.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://twy.xinyue.icu

[S56] C++：optional
来源：http://ctn.cashguo.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wty.hammf.cn

[S57] C++：编译期常量
来源：http://uqj.zhongyouzk.top

constexpr int N = 10;
来源：http://phd.ehwqpu.com

[S58] C++：命名空间
来源：http://ydz.quarkkingdee.top

namespace ns { int f() { return 1; } }
来源：http://zxz.tarul.cn

[S59] C++：静态断言
来源：http://mpx.9152youxi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eaq.yangfankeji.com

[S60] C++：遍历并删除元素
来源：http://dga.zhixingplan.top


<!-- 参考信息 -->