代发 wailian999

[Q82] 字符长度与字节长度
来源：http://pcu.zdbjq.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ilh.zhaomingkeji.xyz

[Q83] 大小写转换
来源：http://agr.tarul.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://byj.nanxinkj.top

[Q84] 去除首尾空格
来源：http://djy.hfpthk.cn

SELECT TRIM(name) FROM users;
来源：http://ktm.zhoulong.xyz

[Q85] 数值取整
来源：http://irb.jinqigufen.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rus.birdmap.top

[Q86] 读取 JSON 字段
来源：http://ehi.nwbrower.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vyp.svipenyu.cn

[Q87] JSON 字段做条件
来源：http://nmw.hcnkem.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fpq.xuetiantiany.cn

[Q88] 行转列（条件聚合）
来源：http://wff.52xcode.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rjn.cucudq.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wea.tian-w.cn

[Q89] 判断表是否存在
来源：http://vew.yfazqb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ohg.snrcjt.cn

[Q90] 生成序号列
来源：http://ntv.tianlin.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jwb.xziqi.cn

================================================================================
来源：http://ubt.tarul.cn

R. Bash 专题
来源：http://pah.daxiang520.top

================================================================================
来源：http://erc.jinyuanbaomall.cn

[R01] shebang 与严格模式
来源：http://gdt.zhongyouzk.top

#!/usr/bin/env bash
来源：http://kqm.hywenlv.cn

set -euo pipefail
来源：http://ujf.zhengqikj.top

[R02] 变量赋值与使用
来源：http://tri.shanyushiyangkeji.top

name="Tom"; echo "$name"
来源：http://xsw.cdnleiting.top

[R03] 只读变量
来源：http://qtv.guowangkeji.top

readonly PI=3.14
来源：http://rzm.xingfuxueyuan.xyz

[R04] 位置参数
来源：http://woa.xylfe.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ofy.ivvv.top

[R05] 参数默认值
来源：http://rtg.mhx1999.top

name="${1:-default}"
来源：http://gov.yj20258.top

[R06] 判断命令是否存在
来源：http://syi.dianchejie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ubr.mhx1999.top

[R07] if 判断文件
来源：http://dyr.zhoulong.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://slf.snrcjt.cn

[R08] 数值比较
来源：http://sdv.yanxiufei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bvj.shangyingyoupin.top

[R09] 字符串比较
来源：http://rxy.0kj1m.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xpy.shuidangran.top

[R10] 正则匹配
来源：http://fiw.316326.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://won.dashuyun.cn

[R11] case 多分支
来源：http://gxt.guannengcc.top

case "$1" in
来源：http://cvx.xuanzx.com

start) echo "启动" ;;
来源：http://klw.guowangkeji.top

stop)  echo "停止" ;;
来源：http://mjy.zhiwuduotai.top

*)     echo "未知命令" ;;
来源：http://ysd.guannengcc.top

esac
来源：http://lcr.smart0.xyz

[R12] for 遍历文件
来源：http://fkh.zhijiandao.cn

for f in *.txt; do echo "$f"; done
来源：http://fah.guowangkeji.top

[R13] for 计数循环
来源：http://osc.shanyushiyangtech.top

for i in {1..10}; do echo "$i"; done
来源：http://bin.yuanzhike.top

[R14] C 风格 for
来源：http://aza.xuetiantiany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wec.fzhhl.top

[R15] while 逐行读文件
来源：http://jdh.jinqigufen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xkm.fengsongda.top

[R16] until 等待条件
来源：http://zoh.hnqzz.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pjh.aibaodan.cn

[R17] 数组定义与取值
来源：http://ljd.ybcxt.top

arr=(a b c); echo "${arr[0]}"
来源：http://uml.hcnkem.com

[R18] 遍历数组
来源：http://rkl.9152youxi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xoz.sweek.top

[R19] 数组长度
来源：http://vof.xinyue.icu

echo "${#arr[@]}"
来源：http://lfz.redwolf501.top

[R20] 关联数组（字典）
来源：http://fkb.sjlbkw.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lbz.jinqigufen.top

[R21] 字符串长度
来源：http://ozz.chenlongwang.top

echo "${#s}"
来源：http://dmt.aibaodan.cn

[R22] 截取子串
来源：http://egi.snrcjt.cn

echo "${s:0:5}"
来源：http://lpi.jqgufenzy.top

[R23] 字符串替换
来源：http://wdp.wangshuangyany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wib.hnxiangtu.top

[R24] 大小写转换
来源：http://yea.wangdashe.top

echo "${s^^}"; echo "${s,,}"
来源：http://qam.tanke756.top

[R25] 去后缀 / 去前缀
来源：http://jro.c1oappe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://qzn.guannengcc.top

[R26] 命令替换
来源：http://dfi.52xcode.cn

now=$(date +%F); echo "$now"
来源：http://hyq.hfpthk.cn

[R27] 算术展开
来源：http://ril.aibaodan.cn

echo $((1 + 2 * 3))
来源：http://ala.chenlongwang.top

[R28] 浮点运算
来源：http://bpe.jlsjyb.cn

echo "scale=2; 10/3" | bc
来源：http://wsq.ctjpmb.com

[R29] 定义函数
来源：http://swx.yonumen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xjz.ppjwa.cn

[R30] 函数返回状态码
来源：http://yxz.aibaodan.cn

f() { return 0; }; f || echo "失败了"
来源：http://ztw.guowangkeji.top

[R31] 局部变量
来源：http://aaz.fzhhl.top

f() { local x=1; echo "$x"; }
来源：http://zqx.shuidangran.top

[R32] 参数个数校验
来源：http://yjx.hfpthk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qkb.zdbjq.cn

[R33] 捕获错误并提示行号
来源：http://kns.havefunace.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pec.andypj.xyz

[R34] 退出时清理
来源：http://ttt.tianlin.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://nyg.iojbl.cn

[R35] 后台执行并等待
来源：http://bpb.hfpthk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vuu.c1oappe.top

[R36] 并发执行多个任务
来源：http://mom.c1oappe.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://urm.chenjidiqi.icu

[R37] 把输出赋给变量
来源：http://fcb.svipenyu.cn

files=$(ls -1)
来源：http://cot.yvedp.cn

[R38] 管道串联
来源：http://lja.havefunace.top

cat a.txt | grep -i error | wc -l
来源：http://eci.gzhubu.top

[R39] 重定向标准输出与错误
来源：http://did.aizwys.cn

cmd > out.log 2>&1
来源：http://hae.yuxming.cn

[R40] 追加写日志
来源：http://wpb.birdmap.top

echo "log" >> out.log
来源：http://gze.gzhubu.top

[R41] 丢弃输出
来源：http://hde.yj202588.top

cmd >/dev/null 2>&1
来源：http://klv.yuxming.cn

[R42] 输入重定向
来源：http://jkd.shangyingyoupin.top

wc -l < a.txt
来源：http://dtr.gzhubu.top

[R43] 按名字查找文件
来源：http://mhw.pycfn.com

find . -name "*.log" -type f
来源：http://vcf.ywan-chungtsiang.top

[R44] 按修改时间查找
来源：http://gvw.dashuyun.cn

find . -mtime -7 -type f
来源：http://msg.shuidangran.top

[R45] 批量删除
来源：http://vho.iojbl.cn

find . -name "*.tmp" -delete
来源：http://yab.jqgfzy.top

[R46] 递归替换文件内容
来源：http://ldz.svipenyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://alk.yfazqb.com

[R47] sed 单行替换
来源：http://uyy.hfpthk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ewm.wangdashe.top

[R48] awk 取指定列
来源：http://aya.gzhubu.top

awk '{print $1, $3}' a.txt
来源：http://oek.tian-w.cn

[R49] awk 带条件
来源：http://iyh.hnxiangtu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bzy.fehbvm.com

[R50] awk 求和
来源：http://tln.guannengcc.top

awk '{s += $2} END {print s}' a.txt
来源：http://htz.zhoulong.xyz

[R51] 排序去重取前几
来源：http://nme.iojbl.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gxx.jinqigufen.top

[R52] 统计行数
来源：http://pox.hysaishi.cn

wc -l a.txt
来源：http://shb.hfpthk.cn

[R53] 查看文件头与实时尾
来源：http://sis.ctjpmb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ubf.jqgufenzy.top

[R54] 比较两个文件
来源：http://vvy.yueranfly.top

diff a.txt b.txt
来源：http://xkp.zdqjudy.top

[R55] 压缩与解压
来源：http://cdm.epnwcf.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rhc.gzhubu.top

[R56] 远程拷贝
来源：http://kor.hcnkem.com

scp file user@host:/path/
来源：http://mut.yueranfly.top

[R57] 远程执行命令
来源：http://gte.birdmap.top

ssh user@host 'uptime'
来源：http://qfp.nwbrower.top

[R58] 下载文件
来源：http://gmp.vqdsnc.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kvz.zhengqikj.top

[R59] 发 POST JSON
来源：http://eou.smart0.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nzx.guannengcc.top

[R60] 只看 HTTP 状态码
来源：http://xdb.hysaishi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://agt.316326.xyz

[R61] 磁盘占用
来源：http://nrb.fanxiaobao.xyz

df -h;  du -sh *
来源：http://xrr.gotoacloud.top

[R62] 找最占空间的文件
来源：http://mrw.tanke756.top

du -ah . | sort -rh | head -10
来源：http://huq.guannengcc.top

[R63] 内存与进程
来源：http://etz.ctjpmb.com

free -h;  ps aux | grep nginx
来源：http://wiq.hnqzz.top

[R64] 结束进程
来源：http://rxu.xinyue.icu

kill -9 $(pgrep -f app.py)
来源：http://qqw.fehbvm.com

[R65] 查看端口占用
来源：http://pgp.zycfv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ulg.yuanzhike.top

[R66] 定时任务
来源：http://vjy.ybcxt.top

crontab -e;  crontab -l
来源：http://lix.sweek.top

[R67] 生成随机十六进制串
来源：http://smj.yueranfly.top

openssl rand -hex 16
来源：http://ifi.guannengcc.top

[R68] 计算文件校验值
来源：http://jci.tian-w.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hvd.yuxming.cn

[R69] 生成随机密码
来源：http://gmj.gaohongyu789.top

head -c 16 /dev/urandom | base64
来源：http://rlb.pengpengdd.cyou

[R70] 时间戳与互转
来源：http://dkj.yueranfly.top

date +%s;  date -d @1700000000
来源：http://dqr.fehbvm.com

[R71] 日期格式化
来源：http://jam.snrcjt.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cnb.hnxiangtu.top

[R72] 等待端口就绪
来源：http://rkj.pengpengdd.cyou

until nc -z localhost 3306; do sleep 1; done
来源：http://hdj.fehbvm.com

[R73] 分割大日志
来源：http://tlz.meibo888.top

split -l 1000 big.log part_
来源：http://phm.birdmap.top

[R74] 批量重命名
来源：http://bjo.hnxiangtu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jtn.jqgufenzy.top

[R75] 导出环境变量
来源：http://ndi.dianchejie.cn

export PATH="$HOME/bin:$PATH"
来源：http://huc.ywan-chungtsiang.top

[R76] 使用临时文件
来源：http://msu.xuetiantiany.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ltj.xingfuxueyuan.xyz

[R77] 读取用户输入
来源：http://lha.bjfxy.top

read -rp "请输入: " ans
来源：http://xuv.fktsv.cn

[R78] 交互式菜单
来源：http://zag.zhixingplan.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qfw.jinqigufen.top

[R79] 解析命令行选项
来源：http://elw.bjfxy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://upz.316326.xyz

[R80] 查看脚本执行耗时
来源：http://eay.sufxvd.cn

time ./run.sh
来源：http://phg.shzxlz.cn

================================================================================
来源：http://cfw.uphjek.com

S. C / C++ 专题
来源：http://mdv.shanyushiyangkeji.top

================================================================================
来源：http://dhe.yj20258.top

[S01] C：Hello World
来源：http://tnj.quarkkingdee.top

#include <stdio.h>
来源：http://nbu.ivvv.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rnd.cashguo.top

[S02] C：变量与格式化输出
来源：http://vqy.yj202588.top

int a = 10; printf("%d\n", a);
来源：http://hqt.ywan-chungtsiang.top

[S03] C：读入整数
来源：http://sbu.9152youxi.cn

int x; scanf("%d", &x);
来源：http://mvn.jyoumei.cn

[S04] C：字符串复制
来源：http://vou.tian-w.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xql.mhx1999.top

[S05] C：字符串长度
来源：http://qej.pycfn.com

strlen(s)
来源：http://zlc.havefunace.top

[S06] C：字符串比较
来源：http://ypp.zdbjq.cn

strcmp(a, b) == 0
来源：http://lyf.ydzc1.top

[S07] C：数组遍历求和
来源：http://ucu.yangfankeji.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mjr.iojbl.cn

[S08] C：动态内存分配与释放
来源：http://hbn.jinghuilouyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qah.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://cxu.xuetiantiany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tpw.guannengcc.top

[S10] C：指针与解引用
来源：http://ypl.daxiang520.top

int *p = &a;  *p = 5;
来源：http://pzq.9152youxi.cn

[S11] C：逐行读文件
来源：http://wrd.yongpay.top

FILE *f = fopen("a.txt", "r");
来源：http://gkw.birdmap.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kkr.zhoulong.xyz

fclose(f);
来源：http://kgv.zhengqikj.top

[S12] C：写文件
来源：http://avq.pycfn.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://unt.yongpay.top

[S13] C：宏定义
来源：http://xmg.jiagoushi.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dbg.gogol.net.cn

[S14] C：枚举
来源：http://alq.ivvv.top

enum Color { RED, GREEN, BLUE };
来源：http://xlu.hysaishi.cn

[S15] C：类型转换
来源：http://gqw.bbcook.cn

(double) a / b
来源：http://cfz.zycfv.cn

[S16] C：位操作置位
来源：http://jdo.tian-w.cn

x |= (1 << 3);
来源：http://exy.yfazqb.com

[S17] C：安全拼接字符串
来源：http://zys.yanxiufei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dvv.tianlin.xyz

[S18] C：命令行参数
来源：http://rox.nanxuanxn.top

int main(int argc, char **argv)
来源：http://emc.tianlin.xyz

[S19] C：快速排序
来源：http://qic.sjlbkw.cn

qsort(a, n, sizeof(int), cmp);
来源：http://beb.hammf.cn

[S20] C：二分查找
来源：http://cgg.zhixingplan.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ddy.zdqjudy.top

[S21] C：字符类别判断
来源：http://wil.jinqigufen.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ega.wangshuangyany.cn

[S22] C：字符串转数字
来源：http://xnw.svipenyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://epf.zhaomingkeji.xyz

[S23] C：随机数
来源：http://mwn.tian-w.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jtu.xuetiantiany.cn

[S24] C：获取本地时间
来源：http://qit.meibo888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tae.yvedp.cn

[S25] C：内存拷贝
来源：http://xgg.dianchejie.cn

memcpy(dst, src, n);
来源：http://tfz.mhx1999.top

[S26] C：内存清零
来源：http://rxv.yfazqb.com

memset(a, 0, sizeof a);
来源：http://jtj.ctjpmb.com

[S27] C：定义常量
来源：http://uie.wangdashe.top

const double PI = 3.14159;
来源：http://ylb.haohaochexian.top

[S28] C：静态变量
来源：http://uwh.yuxming.cn

static int counter = 0;
来源：http://fye.daria6918.cn

[S29] C：变参函数
来源：http://uua.hesvh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ibi.birdmap.top

[S30] C：头文件保护
来源：http://uoj.xziqi.cn

#ifndef X_H
来源：http://lev.sysykeji.top

#define X_H
来源：http://mkm.xziqi.cn

#endif
来源：http://dzv.tianlin.xyz

[S31] C++：Hello World
来源：http://tde.jqgfzy.top

#include <iostream>
来源：http://lei.sxryk.cn

int main() { std::cout << "Hello\n"; }
来源：http://jsm.jinyuanbaomall.cn

[S32] C++：字符串
来源：http://vgb.feifeiyinyue.top

std::string s = "hi";  s += "!";
来源：http://rkb.xziqi.cn

[S33] C++：vector 增删
来源：http://aqx.tianlin.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ujz.redwolf501.top

[S34] C++：遍历 vector
来源：http://zzl.xziqi.cn

for (auto &x : v) { std::cout << x; }
来源：http://lgo.wangdashe.top

[S35] C++：map
来源：http://nme.xziqi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://miu.jinyuanbaomall.cn

[S36] C++：unordered_map
来源：http://isq.xziqi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ahd.yj20258.top

[S37] C++：set
来源：http://mty.jiagoushi.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mar.xylfe.cn

[S38] C++：排序
来源：http://rny.cashguo.top

std::sort(v.begin(), v.end());
来源：http://rdw.bbcook.cn

[S39] C++：自定义比较器排序
来源：http://xdy.yueranfly.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dim.yanxiufei.cn

[S40] C++：查找元素
来源：http://weq.zhixingplan.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uxs.fanxiaobao.xyz

[S41] C++：类与构造函数
来源：http://wes.chenjidiqi.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yre.snrcjt.cn

[S42] C++：继承与虚函数
来源：http://ivp.yanxiufei.cn

class B : public Base { public: void f() override {} };
来源：http://pis.jinqigufen.top

[S43] C++：智能指针
来源：http://lls.xingfuxueyuan.xyz

auto p = std::make_unique<int>(5);
来源：http://usb.ctjpmb.com

[S44] C++：引用传参
来源：http://rme.ydzc1.top

void inc(int &x) { ++x; }
来源：http://pye.shanyushiyangkeji.top

[S45] C++：lambda
来源：http://bty.aizwys.cn

auto add = [](int a, int b) { return a + b; };
来源：http://msy.birdmap.top

[S46] C++：函数模板
来源：http://gdu.nwbrower.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ooa.tarul.cn

[S47] C++：结构化绑定遍历
来源：http://imf.tianlin.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fdv.chenjidiqi.icu

[S48] C++：逐行读文件
来源：http://cez.zhaomingkeji.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://dwi.hywenlv.cn

while (std::getline(in, line)) { }
来源：http://izw.tanke756.top

[S49] C++：写文件
来源：http://gln.hcnkem.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ckw.zdbjq.cn

[S50] C++：格式化数字
来源：http://fqe.ybcxt.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qnx.9152youxi.cn

[S51] C++：显式类型转换
来源：http://cgd.daria6918.cn

static_cast<double>(a) / b
来源：http://emv.nanxuanxn.top

[S52] C++：const 与 noexcept
来源：http://exi.jqgufenzy.top


<!-- 参考信息 -->