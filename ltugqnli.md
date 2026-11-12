代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fbc.0kj1m.cn

[Q90] 生成序号列
来源：http://gvr.vehdjk.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vxq.feifeiyinyue.top

================================================================================
来源：http://ucn.jiagoushi.top

R. Bash 专题
来源：http://pej.shangyingyoupin.top

================================================================================
来源：http://qgt.cashguo.top

[R01] shebang 与严格模式
来源：http://czl.yuxming.cn

#!/usr/bin/env bash
来源：http://ozm.jinghuilouyu.cn

set -euo pipefail
来源：http://ppe.sysykeji.top

[R02] 变量赋值与使用
来源：http://rvx.pycfn.com

name="Tom"; echo "$name"
来源：http://dir.fktsv.cn

[R03] 只读变量
来源：http://rwh.zhaomingkeji.xyz

readonly PI=3.14
来源：http://qaz.ivvv.top

[R04] 位置参数
来源：http://kvc.jqgufenzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://amc.tanke756.top

[R05] 参数默认值
来源：http://eto.hcnkem.com

name="${1:-default}"
来源：http://smt.ydzc1.top

[R06] 判断命令是否存在
来源：http://roc.xuanzx.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lbp.zhijiandao.cn

[R07] if 判断文件
来源：http://hfa.zhengqikj.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ztr.cashguo.top

[R08] 数值比较
来源：http://zat.xingfuxueyuan.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://sdn.zhaomingkeji.xyz

[R09] 字符串比较
来源：http://shi.xylfe.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bse.0kj1m.cn

[R10] 正则匹配
来源：http://wtn.ydzc1.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://aws.zhoulong.xyz

[R11] case 多分支
来源：http://ddg.gotoacloud.top

case "$1" in
来源：http://uqw.xuetiantiany.cn

start) echo "启动" ;;
来源：http://cms.dianchejie.cn

stop)  echo "停止" ;;
来源：http://ygd.jqgfzy.top

*)     echo "未知命令" ;;
来源：http://kha.jianghu66.top

esac
来源：http://cnt.52xcode.cn

[R12] for 遍历文件
来源：http://isw.feifeiyinyue.top

for f in *.txt; do echo "$f"; done
来源：http://jaj.yj202588.top

[R13] for 计数循环
来源：http://uln.iojbl.cn

for i in {1..10}; do echo "$i"; done
来源：http://mhz.zdqjudy.top

[R14] C 风格 for
来源：http://xef.cheryme.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fzi.bbcook.cn

[R15] while 逐行读文件
来源：http://luh.ybcxt.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jsi.guowangkeji.top

[R16] until 等待条件
来源：http://lzu.havefunace.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pjn.mhx1999.top

[R17] 数组定义与取值
来源：http://wva.redwolf501.top

arr=(a b c); echo "${arr[0]}"
来源：http://xgu.yanxiufei.cn

[R18] 遍历数组
来源：http://obt.52xcode.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ktq.nanxuanxn.top

[R19] 数组长度
来源：http://app.sjlbkw.cn

echo "${#arr[@]}"
来源：http://lfy.ehwqpu.com

[R20] 关联数组（字典）
来源：http://tsq.meibo888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kny.yj20258888.top

[R21] 字符串长度
来源：http://yof.andypj.xyz

echo "${#s}"
来源：http://zlc.redwolf501.top

[R22] 截取子串
来源：http://drh.jinyuanbaomall.cn

echo "${s:0:5}"
来源：http://wrc.shangyingyoupin.top

[R23] 字符串替换
来源：http://djq.hfpthk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dni.cashguo.top

[R24] 大小写转换
来源：http://egy.hywenlv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cbv.yfazqb.com

[R25] 去后缀 / 去前缀
来源：http://osy.wangshuangyany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://eoo.feifeiyinyue.top

[R26] 命令替换
来源：http://qpv.zycfv.cn

now=$(date +%F); echo "$now"
来源：http://aja.chenjidiqi.icu

[R27] 算术展开
来源：http://jnu.bjfxy.top

echo $((1 + 2 * 3))
来源：http://bdu.svipenyu.cn

[R28] 浮点运算
来源：http://scz.smart0.xyz

echo "scale=2; 10/3" | bc
来源：http://uex.ppjwa.cn

[R29] 定义函数
来源：http://fda.ybcxt.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eii.shuidangran.top

[R30] 函数返回状态码
来源：http://uih.chenlongwang.top

f() { return 0; }; f || echo "失败了"
来源：http://xki.0kj1m.cn

[R31] 局部变量
来源：http://xps.epnwcf.com

f() { local x=1; echo "$x"; }
来源：http://osv.jqgufenzy.top

[R32] 参数个数校验
来源：http://nau.gotoacloud.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sfy.yj20258.top

[R33] 捕获错误并提示行号
来源：http://nrd.yfazqb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sao.ybcxt.top

[R34] 退出时清理
来源：http://ddb.zhixingplan.top

trap 'rm -f "$tmp"' EXIT
来源：http://uqr.hnxiangtu.top

[R35] 后台执行并等待
来源：http://psi.zhijiandao.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://knh.jinghuilouyu.cn

[R36] 并发执行多个任务
来源：http://iiw.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gnj.cucudq.cn

[R37] 把输出赋给变量
来源：http://tbh.jinghuilouyu.cn

files=$(ls -1)
来源：http://rlc.sweek.top

[R38] 管道串联
来源：http://gog.yj20258888.top

cat a.txt | grep -i error | wc -l
来源：http://ejq.yueranfly.top

[R39] 重定向标准输出与错误
来源：http://isr.yuxming.cn

cmd > out.log 2>&1
来源：http://gxy.ivvv.top

[R40] 追加写日志
来源：http://cuu.jlsjyb.cn

echo "log" >> out.log
来源：http://jjp.dianchejie.cn

[R41] 丢弃输出
来源：http://vay.feifeiyinyue.top

cmd >/dev/null 2>&1
来源：http://lew.sufxvd.cn

[R42] 输入重定向
来源：http://kzi.xinyue.icu

wc -l < a.txt
来源：http://hbb.cheryme.top

[R43] 按名字查找文件
来源：http://kww.yj20258.top

find . -name "*.log" -type f
来源：http://ovt.zycfv.cn

[R44] 按修改时间查找
来源：http://tgn.pengpengdd.cyou

find . -mtime -7 -type f
来源：http://cdn.jyoumei.cn

[R45] 批量删除
来源：http://lws.bbcook.cn

find . -name "*.tmp" -delete
来源：http://chf.yanxiufei.cn

[R46] 递归替换文件内容
来源：http://xoh.yvedp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://alj.ydzc1.top

[R47] sed 单行替换
来源：http://wwu.nanxuanxn.top

sed -i 's/foo/bar/g' a.txt
来源：http://mha.snrcjt.cn

[R48] awk 取指定列
来源：http://pbg.cheryme.top

awk '{print $1, $3}' a.txt
来源：http://lgf.xingfuxueyuan.xyz

[R49] awk 带条件
来源：http://heg.zhongyouzk.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sep.zhijiandao.cn

[R50] awk 求和
来源：http://ada.xinyue.icu

awk '{s += $2} END {print s}' a.txt
来源：http://lgt.dianchejie.cn

[R51] 排序去重取前几
来源：http://vsk.feifeiyinyue.top

sort a.txt | uniq -c | sort -rn | head
来源：http://aim.tanke756.top

[R52] 统计行数
来源：http://nbo.sufxvd.cn

wc -l a.txt
来源：http://mpz.chenzaomai.com

[R53] 查看文件头与实时尾
来源：http://wrp.pycfn.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jeg.hysaishi.cn

[R54] 比较两个文件
来源：http://ccz.xuanzx.com

diff a.txt b.txt
来源：http://tif.sysykeji.top

[R55] 压缩与解压
来源：http://fsr.sysykeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mdx.tianlin.xyz

[R56] 远程拷贝
来源：http://snp.hnxiangtu.top

scp file user@host:/path/
来源：http://jdv.shuidangran.top

[R57] 远程执行命令
来源：http://ryk.yvedp.cn

ssh user@host 'uptime'
来源：http://rfo.cqqwz.cn

[R58] 下载文件
来源：http://bug.tian-w.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jrl.zhengqikj.top

[R59] 发 POST JSON
来源：http://vul.wangshuangyany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eta.epnwcf.com

[R60] 只看 HTTP 状态码
来源：http://tjh.sxryk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zes.fengsongda.top

[R61] 磁盘占用
来源：http://yfx.sysykeji.top

df -h;  du -sh *
来源：http://jip.cashguo.top

[R62] 找最占空间的文件
来源：http://cfc.guowangkeji.top

du -ah . | sort -rh | head -10
来源：http://eyd.svipenyu.cn

[R63] 内存与进程
来源：http://jrw.quarkkingdee.top

free -h;  ps aux | grep nginx
来源：http://zzo.hammf.cn

[R64] 结束进程
来源：http://efq.hesvh.cn

kill -9 $(pgrep -f app.py)
来源：http://wys.nanxinkj.top

[R65] 查看端口占用
来源：http://mtu.ybcxt.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://los.yonumen.top

[R66] 定时任务
来源：http://idn.nanxuanxn.top

crontab -e;  crontab -l
来源：http://nzm.ppjwa.cn

[R67] 生成随机十六进制串
来源：http://sbn.tarul.cn

openssl rand -hex 16
来源：http://hwy.pycfn.com

[R68] 计算文件校验值
来源：http://ffo.guowangkeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://dyf.xingfuxueyuan.xyz

[R69] 生成随机密码
来源：http://lry.wangdashe.top

head -c 16 /dev/urandom | base64
来源：http://yiy.snrcjt.cn

[R70] 时间戳与互转
来源：http://eez.cdnleiting.top

date +%s;  date -d @1700000000
来源：http://aec.redwolf501.top

[R71] 日期格式化
来源：http://mha.zhijiandao.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pni.dashuyun.cn

[R72] 等待端口就绪
来源：http://oku.shuidangran.top

until nc -z localhost 3306; do sleep 1; done
来源：http://loo.birdmap.top

[R73] 分割大日志
来源：http://fbl.zhongyouzk.top

split -l 1000 big.log part_
来源：http://piw.jqgfzy.top

[R74] 批量重命名
来源：http://kkl.yanxiufei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mvt.cdnleiting.top

[R75] 导出环境变量
来源：http://ame.xylfe.cn

export PATH="$HOME/bin:$PATH"
来源：http://dan.redwolf501.top

[R76] 使用临时文件
来源：http://kzu.redwolf501.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bvl.jlsjyb.cn

[R77] 读取用户输入
来源：http://pnx.zhixingplan.top

read -rp "请输入: " ans
来源：http://ivx.quarkkingdee.top

[R78] 交互式菜单
来源：http://dbg.xziqi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jwx.yvedp.cn

[R79] 解析命令行选项
来源：http://qts.cashguo.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oja.hongshengwenyu.top

[R80] 查看脚本执行耗时
来源：http://kgx.chenzaomai.com

time ./run.sh
来源：http://lkv.jyoumei.cn

================================================================================
来源：http://tsj.yvedp.cn

S. C / C++ 专题
来源：http://rua.ywan-chungtsiang.top

================================================================================
来源：http://hic.wangshuangyany.cn

[S01] C：Hello World
来源：http://kpr.dianchejie.cn

#include <stdio.h>
来源：http://qdb.zhoulong.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://clx.guannengcc.top

[S02] C：变量与格式化输出
来源：http://ugl.cucudq.cn

int a = 10; printf("%d\n", a);
来源：http://prx.gzhubu.top

[S03] C：读入整数
来源：http://jdy.shangyingyoupin.top

int x; scanf("%d", &x);
来源：http://stm.yueranfly.top

[S04] C：字符串复制
来源：http://zdb.sjlbkw.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ygu.guannengcc.top

[S05] C：字符串长度
来源：http://ypj.yj202588.top

strlen(s)
来源：http://ggr.iojbl.cn

[S06] C：字符串比较
来源：http://dlp.xinyue.icu

strcmp(a, b) == 0
来源：http://bzw.52xcode.cn

[S07] C：数组遍历求和
来源：http://yyh.316326.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vmu.xinyue.icu

[S08] C：动态内存分配与释放
来源：http://bkv.fanxiaobao.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ovr.daxiang520.top

[S09] C：结构体定义与初始化
来源：http://wnj.zhongyouzk.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qyj.wangdashe.top

[S10] C：指针与解引用
来源：http://lak.hfpthk.cn

int *p = &a;  *p = 5;
来源：http://pvx.chenjidiqi.icu

[S11] C：逐行读文件
来源：http://vyy.zhongyouzk.top

FILE *f = fopen("a.txt", "r");
来源：http://usi.ivvv.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qwd.yuxming.cn

fclose(f);
来源：http://zrc.jianghu66.top

[S12] C：写文件
来源：http://fku.vehdjk.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gaa.fzhhl.top

[S13] C：宏定义
来源：http://atj.ppjwa.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xah.sweek.top

[S14] C：枚举
来源：http://zka.yanxiufei.cn

enum Color { RED, GREEN, BLUE };
来源：http://yth.dashuyun.cn

[S15] C：类型转换
来源：http://rbn.iojbl.cn

(double) a / b
来源：http://chg.jlsjyb.cn

[S16] C：位操作置位
来源：http://rxe.cqqwz.cn

x |= (1 << 3);
来源：http://crm.xylfe.cn

[S17] C：安全拼接字符串
来源：http://lce.9152youxi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://feu.ydjk.org.cn

[S18] C：命令行参数
来源：http://dlr.dianchejie.cn

int main(int argc, char **argv)
来源：http://hbq.ivvv.top

[S19] C：快速排序
来源：http://gsi.epnwcf.com

qsort(a, n, sizeof(int), cmp);
来源：http://dle.ydjk.org.cn

[S20] C：二分查找
来源：http://juo.snrcjt.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uvi.mhx1999.top

[S21] C：字符类别判断
来源：http://fcf.sysykeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://npl.yonumen.top

[S22] C：字符串转数字
来源：http://icq.ctjpmb.com

atoi("42");  strtod("3.14", NULL);
来源：http://tge.bbcook.cn

[S23] C：随机数
来源：http://ccm.hongshengwenyu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://tvn.fanxiaobao.xyz

[S24] C：获取本地时间
来源：http://cct.tianlin.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://knb.jqgufenzy.top

[S25] C：内存拷贝
来源：http://qyj.shuidangran.top

memcpy(dst, src, n);
来源：http://vir.shuidangran.top

[S26] C：内存清零
来源：http://gjj.gzhubu.top

memset(a, 0, sizeof a);
来源：http://gop.hnqzz.top

[S27] C：定义常量
来源：http://wwv.guowangkeji.top

const double PI = 3.14159;
来源：http://ssf.uphjek.com

[S28] C：静态变量
来源：http://xka.pycfn.com

static int counter = 0;
来源：http://opc.cucudq.cn

[S29] C：变参函数
来源：http://hgu.sufxvd.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jzp.jqgufenzy.top

[S30] C：头文件保护
来源：http://iww.xuetiantiany.cn

#ifndef X_H
来源：http://ndr.hnqzz.top

#define X_H
来源：http://rtj.fengsongda.top

#endif
来源：http://upl.feifeiyinyue.top

[S31] C++：Hello World
来源：http://qgd.jlsjyb.cn

#include <iostream>
来源：http://dlz.yfazqb.com

int main() { std::cout << "Hello\n"; }
来源：http://afd.cqqwz.cn

[S32] C++：字符串
来源：http://mdn.jlsjyb.cn

std::string s = "hi";  s += "!";
来源：http://rke.fktsv.cn

[S33] C++：vector 增删
来源：http://uil.bbcook.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tog.andypj.xyz

[S34] C++：遍历 vector
来源：http://jzo.xingfuxueyuan.xyz

for (auto &x : v) { std::cout << x; }
来源：http://wba.hammf.cn

[S35] C++：map
来源：http://rod.svipenyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vsn.guowangkeji.top

[S36] C++：unordered_map
来源：http://oju.epnwcf.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vmt.zhijiandao.cn

[S37] C++：set
来源：http://cvu.ppjwa.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ltc.316326.xyz

[S38] C++：排序
来源：http://azf.fehbvm.com

std::sort(v.begin(), v.end());
来源：http://sez.xziqi.cn

[S39] C++：自定义比较器排序
来源：http://ybp.ydjk.org.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blt.c1oappe.top

[S40] C++：查找元素
来源：http://ote.nwbrower.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xon.ywan-chungtsiang.top

[S41] C++：类与构造函数
来源：http://any.cdnleiting.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://crg.shanyushiyangkeji.top

[S42] C++：继承与虚函数
来源：http://hbk.jinyuanbaomall.cn

class B : public Base { public: void f() override {} };
来源：http://lss.yongpay.top

[S43] C++：智能指针
来源：http://vlu.quarkkingdee.top

auto p = std::make_unique<int>(5);
来源：http://ues.yuxming.cn

[S44] C++：引用传参
来源：http://xfu.yangfankeji.com

void inc(int &x) { ++x; }
来源：http://ozc.tarul.cn

[S45] C++：lambda
来源：http://kml.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://csb.pycfn.com

[S46] C++：函数模板
来源：http://zzv.shangyingyoupin.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zfv.fengsongda.top

[S47] C++：结构化绑定遍历
来源：http://zsr.wangdashe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://soo.hesvh.cn

[S48] C++：逐行读文件
来源：http://hhy.ctjpmb.com

std::ifstream in("a.txt");  std::string line;
来源：http://mop.yueranfly.top

while (std::getline(in, line)) { }
来源：http://jkj.kuanghao11.cn

[S49] C++：写文件
来源：http://hpx.sweek.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jfo.yonumen.top

[S50] C++：格式化数字
来源：http://qiu.sweek.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tne.yj20258.top

[S51] C++：显式类型转换
来源：http://wea.9152youxi.cn

static_cast<double>(a) / b
来源：http://kjp.xuetiantiany.cn

[S52] C++：const 与 noexcept
来源：http://xnr.quarkkingdee.top

int size() const noexcept { return n_; }
来源：http://xdo.yvedp.cn

[S53] C++：移动语义
来源：http://bkj.hammf.cn

std::vector<int> w = std::move(v);
来源：http://ygq.havefunace.top

[S54] C++：异常处理
来源：http://zzp.birdmap.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vot.jinyuanbaomall.cn

[S55] C++：结构化绑定
来源：http://xwn.jqgufenzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://scg.yuxming.cn

[S56] C++：optional
来源：http://efn.hesvh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vpe.pengpengdd.cyou

[S57] C++：编译期常量
来源：http://weq.zhengqikj.top

constexpr int N = 10;
来源：http://toz.vqdsnc.cn

[S58] C++：命名空间
来源：http://bsq.fzhhl.top

namespace ns { int f() { return 1; } }
来源：http://evc.pengpengdd.cyou

[S59] C++：静态断言
来源：http://oji.jinghuilouyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kci.tianlin.xyz

[S60] C++：遍历并删除元素
来源：http://kkb.jinghuilouyu.cn


<!-- 参考信息 -->