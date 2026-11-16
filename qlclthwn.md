代发 wailian999

[Q80] 字符串截取
来源：http://sqq.zhoulong.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ukk.zhongyouzk.top

[Q81] 字符串替换
来源：http://cjs.jinghuilouyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://trh.ywan-chungtsiang.top

[Q82] 字符长度与字节长度
来源：http://idu.cdnleiting.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://twp.ivvv.top

[Q83] 大小写转换
来源：http://ogo.yfazqb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sqi.jinqigfzy.top

[Q84] 去除首尾空格
来源：http://mdg.dashuyun.cn

SELECT TRIM(name) FROM users;
来源：http://dye.sweek.top

[Q85] 数值取整
来源：http://qoy.fktsv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rym.jqgufenzy.top

[Q86] 读取 JSON 字段
来源：http://uqk.tian-w.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ymf.gogol.net.cn

[Q87] JSON 字段做条件
来源：http://cfi.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pkk.yonumen.top

[Q88] 行转列（条件聚合）
来源：http://qhr.316326.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uyj.yvedp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://igy.zdbjq.cn

[Q89] 判断表是否存在
来源：http://ody.iojbl.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zpa.shuidangran.top

[Q90] 生成序号列
来源：http://kek.xinyue.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hvr.ehwqpu.com

================================================================================
来源：http://khq.jyoumei.cn

R. Bash 专题
来源：http://pbm.tanke756.top

================================================================================
来源：http://xjs.chenlongwang.top

[R01] shebang 与严格模式
来源：http://dgr.sufxvd.cn

#!/usr/bin/env bash
来源：http://lxt.sufxvd.cn

set -euo pipefail
来源：http://mao.dashuyun.cn

[R02] 变量赋值与使用
来源：http://yfn.redwolf501.top

name="Tom"; echo "$name"
来源：http://hvg.ydjk.org.cn

[R03] 只读变量
来源：http://rfm.xuetiantiany.cn

readonly PI=3.14
来源：http://fdi.svipenyu.cn

[R04] 位置参数
来源：http://vfo.cashguo.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yry.yvedp.cn

[R05] 参数默认值
来源：http://qll.hysaishi.cn

name="${1:-default}"
来源：http://ayi.zhaomingkeji.xyz

[R06] 判断命令是否存在
来源：http://ouo.hongshengwenyu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hhj.bbcook.cn

[R07] if 判断文件
来源：http://udq.cqqwz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nzw.svipenyu.cn

[R08] 数值比较
来源：http://ohu.xziqi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://otk.shzxlz.cn

[R09] 字符串比较
来源：http://lfk.ctjpmb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kfp.wangdashe.top

[R10] 正则匹配
来源：http://ejp.yj20258888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hsn.svipenyu.cn

[R11] case 多分支
来源：http://crp.shangyingyoupin.top

case "$1" in
来源：http://ina.jinyuanbaomall.cn

start) echo "启动" ;;
来源：http://lgj.xingfuxueyuan.xyz

stop)  echo "停止" ;;
来源：http://pyc.andypj.xyz

*)     echo "未知命令" ;;
来源：http://uwb.pycfn.com

esac
来源：http://wup.hammf.cn

[R12] for 遍历文件
来源：http://xgx.epnwcf.com

for f in *.txt; do echo "$f"; done
来源：http://twl.yj20258888.top

[R13] for 计数循环
来源：http://ubg.sxryk.cn

for i in {1..10}; do echo "$i"; done
来源：http://hiv.ivvv.top

[R14] C 风格 for
来源：http://rbj.jinqigfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://arf.tarul.cn

[R15] while 逐行读文件
来源：http://vlz.ywan-chungtsiang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://syx.bjfxy.top

[R16] until 等待条件
来源：http://bog.fzhhl.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eqn.nwbrower.top

[R17] 数组定义与取值
来源：http://xcd.hywenlv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oaf.tarul.cn

[R18] 遍历数组
来源：http://tdg.dashuyun.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://djd.daxiang520.top

[R19] 数组长度
来源：http://quk.aizwys.cn

echo "${#arr[@]}"
来源：http://rmh.wangshuangyany.cn

[R20] 关联数组（字典）
来源：http://qte.uphjek.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rza.c1oappe.top

[R21] 字符串长度
来源：http://umv.zhijiandao.cn

echo "${#s}"
来源：http://uba.ehwqpu.com

[R22] 截取子串
来源：http://ouu.andypj.xyz

echo "${s:0:5}"
来源：http://qzr.hongshengwenyu.top

[R23] 字符串替换
来源：http://vzr.ehwqpu.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://reh.andypj.xyz

[R24] 大小写转换
来源：http://rgn.shzxlz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wbj.jianghu66.top

[R25] 去后缀 / 去前缀
来源：http://tjs.fehbvm.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://jjn.xylfe.cn

[R26] 命令替换
来源：http://duq.kuanghao11.cn

now=$(date +%F); echo "$now"
来源：http://xja.hysaishi.cn

[R27] 算术展开
来源：http://cjv.yfazqb.com

echo $((1 + 2 * 3))
来源：http://izd.fehbvm.com

[R28] 浮点运算
来源：http://iha.hnqzz.top

echo "scale=2; 10/3" | bc
来源：http://xte.xuetiantiany.cn

[R29] 定义函数
来源：http://cnk.iojbl.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qok.xinyue.icu

[R30] 函数返回状态码
来源：http://zek.bbcook.cn

f() { return 0; }; f || echo "失败了"
来源：http://fmo.tian-w.cn

[R31] 局部变量
来源：http://mee.redwolf501.top

f() { local x=1; echo "$x"; }
来源：http://uim.jqgfzy.top

[R32] 参数个数校验
来源：http://kth.wangshuangyany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jjy.xylfe.cn

[R33] 捕获错误并提示行号
来源：http://kqu.uphjek.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://odg.mhx1999.top

[R34] 退出时清理
来源：http://xob.sysykeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://lnt.ybcxt.top

[R35] 后台执行并等待
来源：http://ils.nwbrower.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ewa.yj20258.top

[R36] 并发执行多个任务
来源：http://zpj.shangyingyoupin.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://isz.nwbrower.top

[R37] 把输出赋给变量
来源：http://swi.andypj.xyz

files=$(ls -1)
来源：http://obq.zdqjudy.top

[R38] 管道串联
来源：http://mvj.ydzc1.top

cat a.txt | grep -i error | wc -l
来源：http://hsd.uphjek.com

[R39] 重定向标准输出与错误
来源：http://typ.cashguo.top

cmd > out.log 2>&1
来源：http://pjl.iojbl.cn

[R40] 追加写日志
来源：http://nts.shuidangran.top

echo "log" >> out.log
来源：http://rhx.bjfxy.top

[R41] 丢弃输出
来源：http://jic.ydjk.org.cn

cmd >/dev/null 2>&1
来源：http://cyg.redwolf501.top

[R42] 输入重定向
来源：http://wpx.feifeiyinyue.top

wc -l < a.txt
来源：http://tjf.meibo888.top

[R43] 按名字查找文件
来源：http://yzk.sufxvd.cn

find . -name "*.log" -type f
来源：http://ewa.jinqigufen.top

[R44] 按修改时间查找
来源：http://tkk.ybcxt.top

find . -mtime -7 -type f
来源：http://xxf.yueranfly.top

[R45] 批量删除
来源：http://svi.cdnleiting.top

find . -name "*.tmp" -delete
来源：http://pux.daxiang520.top

[R46] 递归替换文件内容
来源：http://mey.aibaodan.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uhh.jinqigfzy.top

[R47] sed 单行替换
来源：http://krb.havefunace.top

sed -i 's/foo/bar/g' a.txt
来源：http://snm.meibo888.top

[R48] awk 取指定列
来源：http://vkf.shangyingyoupin.top

awk '{print $1, $3}' a.txt
来源：http://nqc.yueranfly.top

[R49] awk 带条件
来源：http://ntf.smart0.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://woe.chenlongwang.top

[R50] awk 求和
来源：http://xcb.yvedp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://orp.jinqigfzy.top

[R51] 排序去重取前几
来源：http://hbd.9152youxi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vfa.andypj.xyz

[R52] 统计行数
来源：http://mhq.nanxuanxn.top

wc -l a.txt
来源：http://mjr.zhijiandao.cn

[R53] 查看文件头与实时尾
来源：http://ryw.sjlbkw.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://krj.xuanzx.com

[R54] 比较两个文件
来源：http://gvu.xingfuxueyuan.xyz

diff a.txt b.txt
来源：http://rhu.hywenlv.cn

[R55] 压缩与解压
来源：http://rbu.snrcjt.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oxg.jiagoushi.top

[R56] 远程拷贝
来源：http://ubh.fanxiaobao.xyz

scp file user@host:/path/
来源：http://xjc.cashguo.top

[R57] 远程执行命令
来源：http://uqq.hnxiangtu.top

ssh user@host 'uptime'
来源：http://xax.cucudq.cn

[R58] 下载文件
来源：http://vot.fanxiaobao.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bqi.jiagoushi.top

[R59] 发 POST JSON
来源：http://dwy.meibo888.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ygx.pengpengdd.cyou

[R60] 只看 HTTP 状态码
来源：http://myu.fehbvm.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bkk.jqgfzy.top

[R61] 磁盘占用
来源：http://jiz.aizwys.cn

df -h;  du -sh *
来源：http://cns.52xcode.cn

[R62] 找最占空间的文件
来源：http://ptk.tarul.cn

du -ah . | sort -rh | head -10
来源：http://ycr.gaohongyu789.top

[R63] 内存与进程
来源：http://ezb.sufxvd.cn

free -h;  ps aux | grep nginx
来源：http://vbb.birdmap.top

[R64] 结束进程
来源：http://sui.yueranfly.top

kill -9 $(pgrep -f app.py)
来源：http://htq.dianchejie.cn

[R65] 查看端口占用
来源：http://apw.sufxvd.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ifs.jqgufenzy.top

[R66] 定时任务
来源：http://ugt.yfazqb.com

crontab -e;  crontab -l
来源：http://pbf.fehbvm.com

[R67] 生成随机十六进制串
来源：http://con.dashuyun.cn

openssl rand -hex 16
来源：http://phk.zdbjq.cn

[R68] 计算文件校验值
来源：http://nvl.zhongyouzk.top

sha256sum a.txt;  md5sum a.txt
来源：http://cvt.zhiwuduotai.top

[R69] 生成随机密码
来源：http://mlm.ppjwa.cn

head -c 16 /dev/urandom | base64
来源：http://rja.xziqi.cn

[R70] 时间戳与互转
来源：http://imf.daxiang520.top

date +%s;  date -d @1700000000
来源：http://mph.meibo888.top

[R71] 日期格式化
来源：http://qyq.jqgufenzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rbw.xziqi.cn

[R72] 等待端口就绪
来源：http://zlr.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://crj.xinyue.icu

[R73] 分割大日志
来源：http://ifn.shzxlz.cn

split -l 1000 big.log part_
来源：http://gpl.hongshengwenyu.top

[R74] 批量重命名
来源：http://uoh.sysykeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pcr.sweek.top

[R75] 导出环境变量
来源：http://tup.xinyue.icu

export PATH="$HOME/bin:$PATH"
来源：http://zyw.bjfxy.top

[R76] 使用临时文件
来源：http://cbs.hysaishi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gzs.dianchejie.cn

[R77] 读取用户输入
来源：http://pom.kuanghao11.cn

read -rp "请输入: " ans
来源：http://mjt.snrcjt.cn

[R78] 交互式菜单
来源：http://rxp.fengsongda.top

select opt in a b c; do echo "$opt"; break; done
来源：http://akq.yj20258888.top

[R79] 解析命令行选项
来源：http://ddg.uphjek.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qgx.cheryme.top

[R80] 查看脚本执行耗时
来源：http://nba.fzhhl.top

time ./run.sh
来源：http://nyp.pycfn.com

================================================================================
来源：http://bua.ivvv.top

S. C / C++ 专题
来源：http://xys.jyoumei.cn

================================================================================
来源：http://hkb.pycfn.com

[S01] C：Hello World
来源：http://bqs.cqqwz.cn

#include <stdio.h>
来源：http://qzz.jqgufenzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ysm.52xcode.cn

[S02] C：变量与格式化输出
来源：http://imn.fehbvm.com

int a = 10; printf("%d\n", a);
来源：http://ctv.shanyushiyangkeji.top

[S03] C：读入整数
来源：http://tfj.andypj.xyz

int x; scanf("%d", &x);
来源：http://cgs.jinqigfzy.top

[S04] C：字符串复制
来源：http://qlq.guowangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://svs.kuanghao11.cn

[S05] C：字符串长度
来源：http://pke.52xcode.cn

strlen(s)
来源：http://aky.yj20258888.top

[S06] C：字符串比较
来源：http://myf.wangshuangyany.cn

strcmp(a, b) == 0
来源：http://ojh.xylfe.cn

[S07] C：数组遍历求和
来源：http://kde.jinqigufen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gkr.yangfankeji.com

[S08] C：动态内存分配与释放
来源：http://njm.jlsjyb.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nkh.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://stl.kuanghao11.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gbs.xingfuxueyuan.xyz

[S10] C：指针与解引用
来源：http://idt.yj20258.top

int *p = &a;  *p = 5;
来源：http://wwb.fehbvm.com

[S11] C：逐行读文件
来源：http://ypc.gogol.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://kco.yuanzhike.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lci.daria6918.cn

fclose(f);
来源：http://prs.yuanzhike.top

[S12] C：写文件
来源：http://vlj.xuetiantiany.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tdm.meibo888.top

[S13] C：宏定义
来源：http://yja.ivvv.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ofu.zhiwuduotai.top

[S14] C：枚举
来源：http://wao.svipenyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://jok.daria6918.cn

[S15] C：类型转换
来源：http://way.fengsongda.top

(double) a / b
来源：http://tkx.cheryme.top

[S16] C：位操作置位
来源：http://wih.zdbjq.cn

x |= (1 << 3);
来源：http://zvg.tanke756.top

[S17] C：安全拼接字符串
来源：http://qaa.uphjek.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ufs.zhongyouzk.top

[S18] C：命令行参数
来源：http://dqi.yj20258888.top

int main(int argc, char **argv)
来源：http://hcm.sweek.top

[S19] C：快速排序
来源：http://jxp.chenjidiqi.icu

qsort(a, n, sizeof(int), cmp);
来源：http://gcs.fzhhl.top

[S20] C：二分查找
来源：http://hwa.cqqwz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wxy.hfpthk.cn

[S21] C：字符类别判断
来源：http://eaa.cqqwz.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yvn.snrcjt.cn

[S22] C：字符串转数字
来源：http://gnc.jianghu66.top

atoi("42");  strtod("3.14", NULL);
来源：http://zso.gotoacloud.top

[S23] C：随机数
来源：http://fxe.iojbl.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wyo.aibaodan.cn

[S24] C：获取本地时间
来源：http://olg.jlsjyb.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rus.jianghu66.top

[S25] C：内存拷贝
来源：http://cxa.ppjwa.cn

memcpy(dst, src, n);
来源：http://dzn.0kj1m.cn

[S26] C：内存清零
来源：http://qrm.yj20258888.top

memset(a, 0, sizeof a);
来源：http://hfg.gzhubu.top

[S27] C：定义常量
来源：http://lxz.guannengcc.top

const double PI = 3.14159;
来源：http://hkh.xinyue.icu

[S28] C：静态变量
来源：http://jdo.haohaochexian.top

static int counter = 0;
来源：http://hdj.quarkkingdee.top

[S29] C：变参函数
来源：http://lyv.sjlbkw.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mte.ivvv.top

[S30] C：头文件保护
来源：http://ehu.yonumen.top

#ifndef X_H
来源：http://lvk.iojbl.cn

#define X_H
来源：http://mlo.chenzaomai.com

#endif
来源：http://cry.jyoumei.cn

[S31] C++：Hello World
来源：http://iqq.zhongyouzk.top

#include <iostream>
来源：http://jio.gzhubu.top

int main() { std::cout << "Hello\n"; }
来源：http://icc.yj202588.top

[S32] C++：字符串
来源：http://psz.tian-w.cn

std::string s = "hi";  s += "!";
来源：http://ldp.epnwcf.com

[S33] C++：vector 增删
来源：http://ggw.9152youxi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dyi.jqgfzy.top

[S34] C++：遍历 vector
来源：http://szc.0kj1m.cn

for (auto &x : v) { std::cout << x; }
来源：http://goa.ivvv.top

[S35] C++：map
来源：http://uxw.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eby.tarul.cn

[S36] C++：unordered_map
来源：http://qqu.cucudq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nob.hywenlv.cn

[S37] C++：set
来源：http://wfn.sjlbkw.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ijz.jlsjyb.cn

[S38] C++：排序
来源：http://tdi.zdqjudy.top

std::sort(v.begin(), v.end());
来源：http://zde.sufxvd.cn

[S39] C++：自定义比较器排序
来源：http://dri.c1oappe.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vtt.yvedp.cn

[S40] C++：查找元素
来源：http://cue.snrcjt.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kqt.chenlongwang.top

[S41] C++：类与构造函数
来源：http://kei.chenlongwang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yia.epnwcf.com

[S42] C++：继承与虚函数
来源：http://use.shzxlz.cn

class B : public Base { public: void f() override {} };
来源：http://ksh.jinqigfzy.top

[S43] C++：智能指针
来源：http://knt.shanyushiyangtech.top

auto p = std::make_unique<int>(5);
来源：http://cid.jianghu66.top

[S44] C++：引用传参
来源：http://dbm.redwolf501.top

void inc(int &x) { ++x; }
来源：http://ynq.hysaishi.cn

[S45] C++：lambda
来源：http://jvm.xziqi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qhu.fzhhl.top

[S46] C++：函数模板
来源：http://jni.meibo888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://emc.hysaishi.cn

[S47] C++：结构化绑定遍历
来源：http://pbx.pycfn.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kjz.feifeiyinyue.top

[S48] C++：逐行读文件
来源：http://cng.yongpay.top

std::ifstream in("a.txt");  std::string line;
来源：http://vmw.fanxiaobao.xyz

while (std::getline(in, line)) { }
来源：http://fgh.shanyushiyangkeji.top

[S49] C++：写文件
来源：http://hrs.ybcxt.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yqc.kuanghao11.cn

[S50] C++：格式化数字
来源：http://opt.ywan-chungtsiang.top


<!-- 参考信息 -->