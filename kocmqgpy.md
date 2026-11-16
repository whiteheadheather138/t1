代发 wailian999

[Q84] 去除首尾空格
来源：http://cfb.zhixingplan.top

SELECT TRIM(name) FROM users;
来源：http://sgx.hfpthk.cn

[Q85] 数值取整
来源：http://ewc.zhixingplan.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://evp.daxiang520.top

[Q86] 读取 JSON 字段
来源：http://ejb.cqqwz.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hif.nanxinkj.top

[Q87] JSON 字段做条件
来源：http://txa.tian-w.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fyq.hnxiangtu.top

[Q88] 行转列（条件聚合）
来源：http://hqr.gotoacloud.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://eqx.shangyingyoupin.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pyo.sysykeji.top

[Q89] 判断表是否存在
来源：http://gjt.jlsjyb.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://txf.ivvv.top

[Q90] 生成序号列
来源：http://jdq.vqdsnc.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jrl.iojbl.cn

================================================================================
来源：http://kei.52xcode.cn

R. Bash 专题
来源：http://uva.shuidangran.top

================================================================================
来源：http://myv.pengpengdd.cyou

[R01] shebang 与严格模式
来源：http://oza.fzhhl.top

#!/usr/bin/env bash
来源：http://kbf.chenlongwang.top

set -euo pipefail
来源：http://ssg.yanxiufei.cn

[R02] 变量赋值与使用
来源：http://rdr.cdnleiting.top

name="Tom"; echo "$name"
来源：http://biv.0kj1m.cn

[R03] 只读变量
来源：http://vzk.fktsv.cn

readonly PI=3.14
来源：http://kde.nwbrower.top

[R04] 位置参数
来源：http://rie.c1oappe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wfd.dashuyun.cn

[R05] 参数默认值
来源：http://xwz.gogol.net.cn

name="${1:-default}"
来源：http://tdt.guowangkeji.top

[R06] 判断命令是否存在
来源：http://hak.ehwqpu.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zvx.0kj1m.cn

[R07] if 判断文件
来源：http://sck.zhiwuduotai.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://llb.havefunace.top

[R08] 数值比较
来源：http://eaw.ehwqpu.com

if (( a > b )); then echo "a 更大"; fi
来源：http://uen.xylfe.cn

[R09] 字符串比较
来源：http://qxp.hywenlv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vbd.quarkkingdee.top

[R10] 正则匹配
来源：http://fve.jianghu66.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gyh.wangdashe.top

[R11] case 多分支
来源：http://pru.chenjidiqi.icu

case "$1" in
来源：http://gws.shzxlz.cn

start) echo "启动" ;;
来源：http://zym.guannengcc.top

stop)  echo "停止" ;;
来源：http://wdl.sufxvd.cn

*)     echo "未知命令" ;;
来源：http://sox.nwbrower.top

esac
来源：http://nil.fanxiaobao.xyz

[R12] for 遍历文件
来源：http://gly.xingfuxueyuan.xyz

for f in *.txt; do echo "$f"; done
来源：http://lkd.yj202588.top

[R13] for 计数循环
来源：http://lxp.jianghu66.top

for i in {1..10}; do echo "$i"; done
来源：http://ams.yj20258.top

[R14] C 风格 for
来源：http://pdd.hesvh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ouc.sysykeji.top

[R15] while 逐行读文件
来源：http://gil.ydzc1.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ava.hfpthk.cn

[R16] until 等待条件
来源：http://kye.yangfankeji.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cqy.fzhhl.top

[R17] 数组定义与取值
来源：http://cdc.shanyushiyangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://epz.hcnkem.com

[R18] 遍历数组
来源：http://efp.cashguo.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zsw.iojbl.cn

[R19] 数组长度
来源：http://cvn.xingfuxueyuan.xyz

echo "${#arr[@]}"
来源：http://apw.nwbrower.top

[R20] 关联数组（字典）
来源：http://vef.sysykeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xav.tanke756.top

[R21] 字符串长度
来源：http://rxn.gogol.net.cn

echo "${#s}"
来源：http://tkn.uphjek.com

[R22] 截取子串
来源：http://jpx.ehwqpu.com

echo "${s:0:5}"
来源：http://thb.havefunace.top

[R23] 字符串替换
来源：http://ueh.ydjk.org.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://plm.aibaodan.cn

[R24] 大小写转换
来源：http://rio.zdqjudy.top

echo "${s^^}"; echo "${s,,}"
来源：http://jmx.yuanzhike.top

[R25] 去后缀 / 去前缀
来源：http://gaa.gogol.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://prq.guannengcc.top

[R26] 命令替换
来源：http://lyr.fanxiaobao.xyz

now=$(date +%F); echo "$now"
来源：http://hui.ctjpmb.com

[R27] 算术展开
来源：http://qty.fehbvm.com

echo $((1 + 2 * 3))
来源：http://tmb.fktsv.cn

[R28] 浮点运算
来源：http://cwy.vehdjk.com

echo "scale=2; 10/3" | bc
来源：http://vda.chenlongwang.top

[R29] 定义函数
来源：http://aal.sxryk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fge.jiagoushi.top

[R30] 函数返回状态码
来源：http://ehe.ctjpmb.com

f() { return 0; }; f || echo "失败了"
来源：http://nmw.yueranfly.top

[R31] 局部变量
来源：http://lsq.jinqigfzy.top

f() { local x=1; echo "$x"; }
来源：http://wox.gogol.net.cn

[R32] 参数个数校验
来源：http://xcm.pengpengdd.cyou

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://whw.andypj.xyz

[R33] 捕获错误并提示行号
来源：http://dow.kuanghao11.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hvz.fengsongda.top

[R34] 退出时清理
来源：http://lnu.wangdashe.top

trap 'rm -f "$tmp"' EXIT
来源：http://god.epnwcf.com

[R35] 后台执行并等待
来源：http://qet.cqqwz.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rlz.cucudq.cn

[R36] 并发执行多个任务
来源：http://pcr.jinyuanbaomall.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://exl.pycfn.com

[R37] 把输出赋给变量
来源：http://vbh.zhiwuduotai.top

files=$(ls -1)
来源：http://iiv.zhengqikj.top

[R38] 管道串联
来源：http://bfa.xziqi.cn

cat a.txt | grep -i error | wc -l
来源：http://nxi.mhx1999.top

[R39] 重定向标准输出与错误
来源：http://ufs.shanyushiyangkeji.top

cmd > out.log 2>&1
来源：http://ysi.chenzaomai.com

[R40] 追加写日志
来源：http://avw.dianchejie.cn

echo "log" >> out.log
来源：http://ege.iojbl.cn

[R41] 丢弃输出
来源：http://uer.jinqigfzy.top

cmd >/dev/null 2>&1
来源：http://ufa.ydjk.org.cn

[R42] 输入重定向
来源：http://sqq.yj202588.top

wc -l < a.txt
来源：http://iex.jlsjyb.cn

[R43] 按名字查找文件
来源：http://ubr.daxiang520.top

find . -name "*.log" -type f
来源：http://tyo.yvedp.cn

[R44] 按修改时间查找
来源：http://egt.hcnkem.com

find . -mtime -7 -type f
来源：http://ing.daria6918.cn

[R45] 批量删除
来源：http://yln.wangdashe.top

find . -name "*.tmp" -delete
来源：http://vnz.yueranfly.top

[R46] 递归替换文件内容
来源：http://hvt.yuxming.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kus.jiagoushi.top

[R47] sed 单行替换
来源：http://qmh.zhaomingkeji.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://lud.sxryk.cn

[R48] awk 取指定列
来源：http://zcm.fanxiaobao.xyz

awk '{print $1, $3}' a.txt
来源：http://naq.sufxvd.cn

[R49] awk 带条件
来源：http://vdt.jinqigfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zau.tian-w.cn

[R50] awk 求和
来源：http://eoj.yongpay.top

awk '{s += $2} END {print s}' a.txt
来源：http://fpd.pycfn.com

[R51] 排序去重取前几
来源：http://jtd.ydzc1.top

sort a.txt | uniq -c | sort -rn | head
来源：http://iqc.hesvh.cn

[R52] 统计行数
来源：http://udx.aizwys.cn

wc -l a.txt
来源：http://egh.yuxming.cn

[R53] 查看文件头与实时尾
来源：http://nzs.fktsv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vgg.jqgufenzy.top

[R54] 比较两个文件
来源：http://yjh.tarul.cn

diff a.txt b.txt
来源：http://sch.jinqigufen.top

[R55] 压缩与解压
来源：http://zwn.shangyingyoupin.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zrm.c1oappe.top

[R56] 远程拷贝
来源：http://auj.birdmap.top

scp file user@host:/path/
来源：http://hxr.yuanzhike.top

[R57] 远程执行命令
来源：http://iyp.smart0.xyz

ssh user@host 'uptime'
来源：http://hlk.tian-w.cn

[R58] 下载文件
来源：http://hpm.mhx1999.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sxx.meibo888.top

[R59] 发 POST JSON
来源：http://hur.yfazqb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ryd.gotoacloud.top

[R60] 只看 HTTP 状态码
来源：http://mwt.fehbvm.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gbx.jqgufenzy.top

[R61] 磁盘占用
来源：http://cod.daria6918.cn

df -h;  du -sh *
来源：http://qsi.zhoulong.xyz

[R62] 找最占空间的文件
来源：http://ryx.cheryme.top

du -ah . | sort -rh | head -10
来源：http://avt.jyoumei.cn

[R63] 内存与进程
来源：http://yyv.yongpay.top

free -h;  ps aux | grep nginx
来源：http://pee.ybcxt.top

[R64] 结束进程
来源：http://lbr.nanxuanxn.top

kill -9 $(pgrep -f app.py)
来源：http://xkz.hongshengwenyu.top

[R65] 查看端口占用
来源：http://bts.epnwcf.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://edg.cdnleiting.top

[R66] 定时任务
来源：http://ljn.ybcxt.top

crontab -e;  crontab -l
来源：http://qcf.ehwqpu.com

[R67] 生成随机十六进制串
来源：http://sfs.kuanghao11.cn

openssl rand -hex 16
来源：http://eic.zycfv.cn

[R68] 计算文件校验值
来源：http://ksk.zhengqikj.top

sha256sum a.txt;  md5sum a.txt
来源：http://edv.nanxuanxn.top

[R69] 生成随机密码
来源：http://xed.c1oappe.top

head -c 16 /dev/urandom | base64
来源：http://oxg.cucudq.cn

[R70] 时间戳与互转
来源：http://yja.hammf.cn

date +%s;  date -d @1700000000
来源：http://aos.xuanzx.com

[R71] 日期格式化
来源：http://dbx.cqqwz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dmv.jiagoushi.top

[R72] 等待端口就绪
来源：http://wzs.ivvv.top

until nc -z localhost 3306; do sleep 1; done
来源：http://neg.vqdsnc.cn

[R73] 分割大日志
来源：http://kvy.jinghuilouyu.cn

split -l 1000 big.log part_
来源：http://khx.nwbrower.top

[R74] 批量重命名
来源：http://jps.guowangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aac.yuanzhike.top

[R75] 导出环境变量
来源：http://wdl.tian-w.cn

export PATH="$HOME/bin:$PATH"
来源：http://kor.jyoumei.cn

[R76] 使用临时文件
来源：http://ndj.snrcjt.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eih.smart0.xyz

[R77] 读取用户输入
来源：http://uud.fzhhl.top

read -rp "请输入: " ans
来源：http://usu.jinghuilouyu.cn

[R78] 交互式菜单
来源：http://jsv.jqgfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tvy.nanxinkj.top

[R79] 解析命令行选项
来源：http://uek.316326.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bxj.gogol.net.cn

[R80] 查看脚本执行耗时
来源：http://zag.xingfuxueyuan.xyz

time ./run.sh
来源：http://own.hnqzz.top

================================================================================
来源：http://tmu.hesvh.cn

S. C / C++ 专题
来源：http://vxj.ydjk.org.cn

================================================================================
来源：http://lma.nwbrower.top

[S01] C：Hello World
来源：http://fbq.yueranfly.top

#include <stdio.h>
来源：http://ayk.aizwys.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vvo.mhx1999.top

[S02] C：变量与格式化输出
来源：http://cjv.guowangkeji.top

int a = 10; printf("%d\n", a);
来源：http://wcw.cucudq.cn

[S03] C：读入整数
来源：http://jik.redwolf501.top

int x; scanf("%d", &x);
来源：http://uyk.guowangkeji.top

[S04] C：字符串复制
来源：http://fyo.hcnkem.com

char dst[32]; strcpy(dst, "hi");
来源：http://tae.52xcode.cn

[S05] C：字符串长度
来源：http://mma.shanyushiyangtech.top

strlen(s)
来源：http://lra.yvedp.cn

[S06] C：字符串比较
来源：http://lvd.yueranfly.top

strcmp(a, b) == 0
来源：http://gzk.gogol.net.cn

[S07] C：数组遍历求和
来源：http://mqv.snrcjt.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zrw.snrcjt.cn

[S08] C：动态内存分配与释放
来源：http://uuw.daria6918.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fzp.ydjk.org.cn

[S09] C：结构体定义与初始化
来源：http://ded.jlsjyb.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xru.zhaomingkeji.xyz

[S10] C：指针与解引用
来源：http://mue.hysaishi.cn

int *p = &a;  *p = 5;
来源：http://qus.iojbl.cn

[S11] C：逐行读文件
来源：http://zqm.haohaochexian.top

FILE *f = fopen("a.txt", "r");
来源：http://bvr.cdnleiting.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vga.wangshuangyany.cn

fclose(f);
来源：http://agd.aizwys.cn

[S12] C：写文件
来源：http://pfv.yanxiufei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://neh.fanxiaobao.xyz

[S13] C：宏定义
来源：http://ssw.c1oappe.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dgb.ydzc1.top

[S14] C：枚举
来源：http://dkw.daria6918.cn

enum Color { RED, GREEN, BLUE };
来源：http://vut.zhengqikj.top

[S15] C：类型转换
来源：http://jyw.bbcook.cn

(double) a / b
来源：http://tdr.jianghu66.top

[S16] C：位操作置位
来源：http://lxg.sufxvd.cn

x |= (1 << 3);
来源：http://mto.sysykeji.top

[S17] C：安全拼接字符串
来源：http://psa.feifeiyinyue.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tjj.mhx1999.top

[S18] C：命令行参数
来源：http://mum.zdqjudy.top

int main(int argc, char **argv)
来源：http://fmp.smart0.xyz

[S19] C：快速排序
来源：http://pos.chenlongwang.top

qsort(a, n, sizeof(int), cmp);
来源：http://yop.zhixingplan.top

[S20] C：二分查找
来源：http://njt.hnxiangtu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qel.shanyushiyangkeji.top

[S21] C：字符类别判断
来源：http://zkl.yuxming.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qlo.sxryk.cn

[S22] C：字符串转数字
来源：http://dke.xuetiantiany.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kzw.fengsongda.top

[S23] C：随机数
来源：http://xnp.gaohongyu789.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jpp.cqqwz.cn

[S24] C：获取本地时间
来源：http://wcx.guowangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://akd.yueranfly.top

[S25] C：内存拷贝
来源：http://sxw.xingfuxueyuan.xyz

memcpy(dst, src, n);
来源：http://iug.gogol.net.cn

[S26] C：内存清零
来源：http://ftj.xziqi.cn

memset(a, 0, sizeof a);
来源：http://ttb.yvedp.cn

[S27] C：定义常量
来源：http://sep.shanyushiyangkeji.top

const double PI = 3.14159;
来源：http://pcf.yj20258888.top

[S28] C：静态变量
来源：http://vah.pengpengdd.cyou

static int counter = 0;
来源：http://gcp.xinyue.icu

[S29] C：变参函数
来源：http://owa.xingfuxueyuan.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ozd.bjfxy.top

[S30] C：头文件保护
来源：http://aqo.wangshuangyany.cn

#ifndef X_H
来源：http://ufl.cashguo.top

#define X_H
来源：http://hak.nanxuanxn.top

#endif
来源：http://jls.bbcook.cn

[S31] C++：Hello World
来源：http://vef.quarkkingdee.top

#include <iostream>
来源：http://dhl.52xcode.cn

int main() { std::cout << "Hello\n"; }
来源：http://cpv.xuetiantiany.cn

[S32] C++：字符串
来源：http://mam.xylfe.cn

std::string s = "hi";  s += "!";
来源：http://oza.316326.xyz

[S33] C++：vector 增删
来源：http://tot.yfazqb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fbu.fktsv.cn

[S34] C++：遍历 vector
来源：http://ttj.gzhubu.top

for (auto &x : v) { std::cout << x; }
来源：http://xwx.tianlin.xyz

[S35] C++：map
来源：http://lls.hnxiangtu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rzp.daria6918.cn

[S36] C++：unordered_map
来源：http://nay.sweek.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ete.tian-w.cn

[S37] C++：set
来源：http://emb.zhongyouzk.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fah.sjlbkw.cn

[S38] C++：排序
来源：http://tli.zhoulong.xyz

std::sort(v.begin(), v.end());
来源：http://ech.jianghu66.top

[S39] C++：自定义比较器排序
来源：http://pdy.dianchejie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jkd.haohaochexian.top

[S40] C++：查找元素
来源：http://cqu.jinqigfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wxe.epnwcf.com

[S41] C++：类与构造函数
来源：http://fyf.hammf.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lpz.shuidangran.top

[S42] C++：继承与虚函数
来源：http://ueb.jqgfzy.top

class B : public Base { public: void f() override {} };
来源：http://osu.xinyue.icu

[S43] C++：智能指针
来源：http://jnv.zhongyouzk.top

auto p = std::make_unique<int>(5);
来源：http://pur.daria6918.cn

[S44] C++：引用传参
来源：http://tdj.tianlin.xyz

void inc(int &x) { ++x; }
来源：http://chx.xuanzx.com

[S45] C++：lambda
来源：http://lox.meibo888.top

auto add = [](int a, int b) { return a + b; };
来源：http://wpe.haohaochexian.top

[S46] C++：函数模板
来源：http://ybp.chenzaomai.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dpr.jqgfzy.top

[S47] C++：结构化绑定遍历
来源：http://eas.nanxinkj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dkl.iojbl.cn

[S48] C++：逐行读文件
来源：http://yqg.hesvh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lfj.fanxiaobao.xyz

while (std::getline(in, line)) { }
来源：http://xlh.316326.xyz

[S49] C++：写文件
来源：http://axh.shanyushiyangtech.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ftc.sjlbkw.cn

[S50] C++：格式化数字
来源：http://bap.zhoulong.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qby.shuidangran.top

[S51] C++：显式类型转换
来源：http://vex.yonumen.top

static_cast<double>(a) / b
来源：http://dht.hnqzz.top

[S52] C++：const 与 noexcept
来源：http://gqz.jqgfzy.top

int size() const noexcept { return n_; }
来源：http://rya.xylfe.cn

[S53] C++：移动语义
来源：http://zmm.fehbvm.com

std::vector<int> w = std::move(v);
来源：http://was.zhongyouzk.top

[S54] C++：异常处理
来源：http://zsx.shangyingyoupin.top


<!-- 参考信息 -->