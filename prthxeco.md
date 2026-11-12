代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ped.xuanzx.com

[Q75] 日期格式化
来源：http://olq.gzhubu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wvm.zhiwuduotai.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://poq.feifeiyinyue.top

[Q76] 按天统计
来源：http://rbf.chenzaomai.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qlg.svipenyu.cn

[Q77] 时间加减
来源：http://mlm.svipenyu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iyz.xylfe.cn

[Q78] 当前时间
来源：http://shw.hcnkem.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yxb.xuanzx.com

[Q79] 字符串拼接
来源：http://tso.zhoulong.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ukd.hnqzz.top

[Q80] 字符串截取
来源：http://gnj.ppjwa.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bre.meibo888.top

[Q81] 字符串替换
来源：http://gmk.gotoacloud.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pto.52xcode.cn

[Q82] 字符长度与字节长度
来源：http://ify.sufxvd.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jpk.zycfv.cn

[Q83] 大小写转换
来源：http://muw.xylfe.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uuv.316326.xyz

[Q84] 去除首尾空格
来源：http://igd.cqqwz.cn

SELECT TRIM(name) FROM users;
来源：http://uyg.316326.xyz

[Q85] 数值取整
来源：http://der.guowangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kik.xuanzx.com

[Q86] 读取 JSON 字段
来源：http://hjl.xylfe.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pdm.ppjwa.cn

[Q87] JSON 字段做条件
来源：http://wzd.vqdsnc.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rrm.feifeiyinyue.top

[Q88] 行转列（条件聚合）
来源：http://nmh.316326.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://way.smart0.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kts.yj202588.top

[Q89] 判断表是否存在
来源：http://hwy.cheryme.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rkd.jqgufenzy.top

[Q90] 生成序号列
来源：http://cfv.shanyushiyangkeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jnp.sweek.top

================================================================================
来源：http://mje.vehdjk.com

R. Bash 专题
来源：http://dub.52xcode.cn

================================================================================
来源：http://ijk.yongpay.top

[R01] shebang 与严格模式
来源：http://arj.fehbvm.com

#!/usr/bin/env bash
来源：http://gfj.xylfe.cn

set -euo pipefail
来源：http://guw.guowangkeji.top

[R02] 变量赋值与使用
来源：http://moo.nanxinkj.top

name="Tom"; echo "$name"
来源：http://xtn.cdnleiting.top

[R03] 只读变量
来源：http://jpz.xingfuxueyuan.xyz

readonly PI=3.14
来源：http://maz.sweek.top

[R04] 位置参数
来源：http://bws.yueranfly.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://grj.zhengqikj.top

[R05] 参数默认值
来源：http://ppl.cucudq.cn

name="${1:-default}"
来源：http://zal.dianchejie.cn

[R06] 判断命令是否存在
来源：http://btt.chenlongwang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fov.jyoumei.cn

[R07] if 判断文件
来源：http://vud.gotoacloud.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kwk.ydzc1.top

[R08] 数值比较
来源：http://axz.hesvh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fyg.316326.xyz

[R09] 字符串比较
来源：http://btk.snrcjt.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bvj.feifeiyinyue.top

[R10] 正则匹配
来源：http://qvv.yj20258888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nxy.yonumen.top

[R11] case 多分支
来源：http://hdv.yuxming.cn

case "$1" in
来源：http://lzg.pycfn.com

start) echo "启动" ;;
来源：http://rnd.tarul.cn

stop)  echo "停止" ;;
来源：http://jsh.daxiang520.top

*)     echo "未知命令" ;;
来源：http://uqs.zdqjudy.top

esac
来源：http://fgv.fanxiaobao.xyz

[R12] for 遍历文件
来源：http://qqd.hammf.cn

for f in *.txt; do echo "$f"; done
来源：http://zzo.chenlongwang.top

[R13] for 计数循环
来源：http://wdw.svipenyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://sos.daria6918.cn

[R14] C 风格 for
来源：http://hmo.feifeiyinyue.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hag.zdbjq.cn

[R15] while 逐行读文件
来源：http://cub.52xcode.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kxf.havefunace.top

[R16] until 等待条件
来源：http://cbt.nwbrower.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://imz.shanyushiyangtech.top

[R17] 数组定义与取值
来源：http://guz.hysaishi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bdv.ppjwa.cn

[R18] 遍历数组
来源：http://vhl.nwbrower.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hdp.jqgfzy.top

[R19] 数组长度
来源：http://cbz.yuanzhike.top

echo "${#arr[@]}"
来源：http://sba.zhaomingkeji.xyz

[R20] 关联数组（字典）
来源：http://kfq.redwolf501.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lur.chenjidiqi.icu

[R21] 字符串长度
来源：http://mgh.gaohongyu789.top

echo "${#s}"
来源：http://ipb.jinqigfzy.top

[R22] 截取子串
来源：http://ozx.aibaodan.cn

echo "${s:0:5}"
来源：http://ovi.fzhhl.top

[R23] 字符串替换
来源：http://qvu.xuetiantiany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aeo.tarul.cn

[R24] 大小写转换
来源：http://cyi.yonumen.top

echo "${s^^}"; echo "${s,,}"
来源：http://hhm.jinqigufen.top

[R25] 去后缀 / 去前缀
来源：http://rgi.zdbjq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://itw.yuanzhike.top

[R26] 命令替换
来源：http://mii.fehbvm.com

now=$(date +%F); echo "$now"
来源：http://oky.zhengqikj.top

[R27] 算术展开
来源：http://kcw.pycfn.com

echo $((1 + 2 * 3))
来源：http://tmc.fehbvm.com

[R28] 浮点运算
来源：http://ewz.wangdashe.top

echo "scale=2; 10/3" | bc
来源：http://del.ydjk.org.cn

[R29] 定义函数
来源：http://wmf.mhx1999.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vvq.jqgufenzy.top

[R30] 函数返回状态码
来源：http://yux.nwbrower.top

f() { return 0; }; f || echo "失败了"
来源：http://klq.uphjek.com

[R31] 局部变量
来源：http://ccg.xuetiantiany.cn

f() { local x=1; echo "$x"; }
来源：http://ktu.chenlongwang.top

[R32] 参数个数校验
来源：http://jfg.jinqigufen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yyy.uphjek.com

[R33] 捕获错误并提示行号
来源：http://fxw.cucudq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bek.aizwys.cn

[R34] 退出时清理
来源：http://kzh.jyoumei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vkb.xuetiantiany.cn

[R35] 后台执行并等待
来源：http://qsm.cheryme.top

sleep 5 & pid=$!; wait "$pid"
来源：http://nbo.cheryme.top

[R36] 并发执行多个任务
来源：http://zvp.chenlongwang.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ehf.guannengcc.top

[R37] 把输出赋给变量
来源：http://vki.0kj1m.cn

files=$(ls -1)
来源：http://ynw.ybcxt.top

[R38] 管道串联
来源：http://obm.9152youxi.cn

cat a.txt | grep -i error | wc -l
来源：http://izd.ppjwa.cn

[R39] 重定向标准输出与错误
来源：http://ksv.chenzaomai.com

cmd > out.log 2>&1
来源：http://cmy.zhengqikj.top

[R40] 追加写日志
来源：http://luj.jqgfzy.top

echo "log" >> out.log
来源：http://oks.yangfankeji.com

[R41] 丢弃输出
来源：http://rst.daxiang520.top

cmd >/dev/null 2>&1
来源：http://vdp.cdnleiting.top

[R42] 输入重定向
来源：http://dsu.vqdsnc.cn

wc -l < a.txt
来源：http://fha.tarul.cn

[R43] 按名字查找文件
来源：http://ngb.nanxinkj.top

find . -name "*.log" -type f
来源：http://thx.zdbjq.cn

[R44] 按修改时间查找
来源：http://jxb.chenlongwang.top

find . -mtime -7 -type f
来源：http://cgr.hnqzz.top

[R45] 批量删除
来源：http://zhh.ywan-chungtsiang.top

find . -name "*.tmp" -delete
来源：http://moy.xuanzx.com

[R46] 递归替换文件内容
来源：http://vsk.zhongyouzk.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cln.aibaodan.cn

[R47] sed 单行替换
来源：http://bjv.dianchejie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dhs.gzhubu.top

[R48] awk 取指定列
来源：http://peq.jinqigfzy.top

awk '{print $1, $3}' a.txt
来源：http://dgc.zhiwuduotai.top

[R49] awk 带条件
来源：http://uan.fehbvm.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wpe.meibo888.top

[R50] awk 求和
来源：http://ogq.cucudq.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cee.ydzc1.top

[R51] 排序去重取前几
来源：http://bzk.haohaochexian.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gfx.jinqigufen.top

[R52] 统计行数
来源：http://nqg.ybcxt.top

wc -l a.txt
来源：http://ono.fehbvm.com

[R53] 查看文件头与实时尾
来源：http://zga.cashguo.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ola.zycfv.cn

[R54] 比较两个文件
来源：http://vsn.xingfuxueyuan.xyz

diff a.txt b.txt
来源：http://jev.jlsjyb.cn

[R55] 压缩与解压
来源：http://akt.xingfuxueyuan.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zic.hesvh.cn

[R56] 远程拷贝
来源：http://eqw.zhaomingkeji.xyz

scp file user@host:/path/
来源：http://vbw.uphjek.com

[R57] 远程执行命令
来源：http://wki.316326.xyz

ssh user@host 'uptime'
来源：http://tim.yj202588.top

[R58] 下载文件
来源：http://iew.chenzaomai.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hyz.0kj1m.cn

[R59] 发 POST JSON
来源：http://jrz.zhengqikj.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qlg.zhaomingkeji.xyz

[R60] 只看 HTTP 状态码
来源：http://xxv.mhx1999.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cin.hcnkem.com

[R61] 磁盘占用
来源：http://awm.andypj.xyz

df -h;  du -sh *
来源：http://vjt.xuetiantiany.cn

[R62] 找最占空间的文件
来源：http://uuq.yanxiufei.cn

du -ah . | sort -rh | head -10
来源：http://hmj.daxiang520.top

[R63] 内存与进程
来源：http://kac.tianlin.xyz

free -h;  ps aux | grep nginx
来源：http://nuh.ywan-chungtsiang.top

[R64] 结束进程
来源：http://lgf.fktsv.cn

kill -9 $(pgrep -f app.py)
来源：http://lqu.sufxvd.cn

[R65] 查看端口占用
来源：http://mxo.0kj1m.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://izv.cheryme.top

[R66] 定时任务
来源：http://vqf.pycfn.com

crontab -e;  crontab -l
来源：http://kpm.guowangkeji.top

[R67] 生成随机十六进制串
来源：http://zrt.jqgufenzy.top

openssl rand -hex 16
来源：http://ito.yj20258.top

[R68] 计算文件校验值
来源：http://all.bjfxy.top

sha256sum a.txt;  md5sum a.txt
来源：http://etn.chenzaomai.com

[R69] 生成随机密码
来源：http://ziv.wangdashe.top

head -c 16 /dev/urandom | base64
来源：http://ugz.wangdashe.top

[R70] 时间戳与互转
来源：http://rul.feifeiyinyue.top

date +%s;  date -d @1700000000
来源：http://uhb.zhengqikj.top

[R71] 日期格式化
来源：http://gwe.xziqi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://amk.vehdjk.com

[R72] 等待端口就绪
来源：http://avp.zdqjudy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hbm.hammf.cn

[R73] 分割大日志
来源：http://hky.nanxinkj.top

split -l 1000 big.log part_
来源：http://qpk.gotoacloud.top

[R74] 批量重命名
来源：http://rnf.316326.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hge.xylfe.cn

[R75] 导出环境变量
来源：http://lwz.jianghu66.top

export PATH="$HOME/bin:$PATH"
来源：http://jql.yj202588.top

[R76] 使用临时文件
来源：http://zjf.fktsv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://giv.zhaomingkeji.xyz

[R77] 读取用户输入
来源：http://zkz.yj202588.top

read -rp "请输入: " ans
来源：http://mln.shanyushiyangtech.top

[R78] 交互式菜单
来源：http://mkk.ivvv.top

select opt in a b c; do echo "$opt"; break; done
来源：http://nan.epnwcf.com

[R79] 解析命令行选项
来源：http://rit.hongshengwenyu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kcz.shuidangran.top

[R80] 查看脚本执行耗时
来源：http://vji.ybcxt.top

time ./run.sh
来源：http://lgm.shangyingyoupin.top

================================================================================
来源：http://krv.smart0.xyz

S. C / C++ 专题
来源：http://kmx.yvedp.cn

================================================================================
来源：http://wkh.yuxming.cn

[S01] C：Hello World
来源：http://roj.wangdashe.top

#include <stdio.h>
来源：http://ddl.sufxvd.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mlx.0kj1m.cn

[S02] C：变量与格式化输出
来源：http://cgz.cqqwz.cn

int a = 10; printf("%d\n", a);
来源：http://rgl.zhijiandao.cn

[S03] C：读入整数
来源：http://wlb.zhengqikj.top

int x; scanf("%d", &x);
来源：http://gvy.wangdashe.top

[S04] C：字符串复制
来源：http://hrl.aizwys.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dqh.cqqwz.cn

[S05] C：字符串长度
来源：http://kme.dianchejie.cn

strlen(s)
来源：http://jtu.jlsjyb.cn

[S06] C：字符串比较
来源：http://znn.0kj1m.cn

strcmp(a, b) == 0
来源：http://yep.chenzaomai.com

[S07] C：数组遍历求和
来源：http://yxp.hongshengwenyu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rpl.316326.xyz

[S08] C：动态内存分配与释放
来源：http://huf.guowangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bvv.ybcxt.top

[S09] C：结构体定义与初始化
来源：http://oac.tian-w.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://srd.dashuyun.cn

[S10] C：指针与解引用
来源：http://yui.tian-w.cn

int *p = &a;  *p = 5;
来源：http://bib.zhengqikj.top

[S11] C：逐行读文件
来源：http://xjl.chenlongwang.top

FILE *f = fopen("a.txt", "r");
来源：http://aye.yuanzhike.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://cew.pengpengdd.cyou

fclose(f);
来源：http://krh.andypj.xyz

[S12] C：写文件
来源：http://vfl.bjfxy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://epj.aibaodan.cn

[S13] C：宏定义
来源：http://uiz.ydjk.org.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cfb.dianchejie.cn

[S14] C：枚举
来源：http://sky.shangyingyoupin.top

enum Color { RED, GREEN, BLUE };
来源：http://gyt.yueranfly.top

[S15] C：类型转换
来源：http://xoa.pengpengdd.cyou

(double) a / b
来源：http://jys.ivvv.top

[S16] C：位操作置位
来源：http://rdm.52xcode.cn

x |= (1 << 3);
来源：http://avy.meibo888.top

[S17] C：安全拼接字符串
来源：http://qmt.shanyushiyangkeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eox.chenzaomai.com

[S18] C：命令行参数
来源：http://ciu.tanke756.top

int main(int argc, char **argv)
来源：http://lsy.zhengqikj.top

[S19] C：快速排序
来源：http://trc.zhaomingkeji.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://kum.tianlin.xyz

[S20] C：二分查找
来源：http://ott.yvedp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uhb.jinqigufen.top

[S21] C：字符类别判断
来源：http://kai.zhengqikj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nhe.sjlbkw.cn

[S22] C：字符串转数字
来源：http://rro.yangfankeji.com

atoi("42");  strtod("3.14", NULL);
来源：http://hmu.zhaomingkeji.xyz

[S23] C：随机数
来源：http://dsv.bbcook.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qqq.hcnkem.com

[S24] C：获取本地时间
来源：http://jup.wangshuangyany.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rln.chenjidiqi.icu

[S25] C：内存拷贝
来源：http://ycl.shanyushiyangtech.top

memcpy(dst, src, n);
来源：http://ktr.ydzc1.top

[S26] C：内存清零
来源：http://tos.guannengcc.top

memset(a, 0, sizeof a);
来源：http://lyn.fzhhl.top

[S27] C：定义常量
来源：http://pad.yonumen.top

const double PI = 3.14159;
来源：http://jkc.cqqwz.cn

[S28] C：静态变量
来源：http://pqv.zhiwuduotai.top

static int counter = 0;
来源：http://ice.yueranfly.top

[S29] C：变参函数
来源：http://xdy.jyoumei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yof.daxiang520.top

[S30] C：头文件保护
来源：http://fof.shzxlz.cn

#ifndef X_H
来源：http://xfl.shanyushiyangkeji.top

#define X_H
来源：http://bio.kuanghao11.cn

#endif
来源：http://fub.shuidangran.top

[S31] C++：Hello World
来源：http://boi.ydjk.org.cn

#include <iostream>
来源：http://ztm.gogol.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://xcr.yanxiufei.cn

[S32] C++：字符串
来源：http://kzh.snrcjt.cn

std::string s = "hi";  s += "!";
来源：http://jeh.ywan-chungtsiang.top

[S33] C++：vector 增删
来源：http://ykc.gotoacloud.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://div.zhixingplan.top

[S34] C++：遍历 vector
来源：http://eim.chenlongwang.top

for (auto &x : v) { std::cout << x; }
来源：http://cbv.vehdjk.com

[S35] C++：map
来源：http://cut.meibo888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ghq.andypj.xyz

[S36] C++：unordered_map
来源：http://ocn.xylfe.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xxl.xuetiantiany.cn

[S37] C++：set
来源：http://ggm.hfpthk.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://woo.birdmap.top

[S38] C++：排序
来源：http://kkz.316326.xyz

std::sort(v.begin(), v.end());
来源：http://jcd.jinghuilouyu.cn

[S39] C++：自定义比较器排序
来源：http://ump.havefunace.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yri.fehbvm.com

[S40] C++：查找元素
来源：http://tqe.wangshuangyany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jch.ydzc1.top

[S41] C++：类与构造函数
来源：http://qys.guowangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://smf.hysaishi.cn

[S42] C++：继承与虚函数
来源：http://nvk.yuanzhike.top

class B : public Base { public: void f() override {} };
来源：http://oxs.jqgfzy.top

[S43] C++：智能指针
来源：http://hsq.dianchejie.cn

auto p = std::make_unique<int>(5);
来源：http://thv.tian-w.cn

[S44] C++：引用传参
来源：http://jif.xylfe.cn

void inc(int &x) { ++x; }
来源：http://lxo.daria6918.cn


<!-- 参考信息 -->