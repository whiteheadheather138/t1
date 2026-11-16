代发 wailian999

ROLLBACK TO sp1;
来源：http://yit.cucudq.cn

[Q69] 查看执行计划
来源：http://djh.wangdashe.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ljf.jinghuilouyu.cn

[Q70] 更新统计信息
来源：http://lsb.c1oappe.top

ANALYZE TABLE users;
来源：http://kwm.ivvv.top

[Q71] 查看建表语句
来源：http://xsq.jinqigfzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sjw.ivvv.top

[Q72] 查看索引
来源：http://uba.pengpengdd.cyou

SHOW INDEX FROM users;
来源：http://kft.feifeiyinyue.top

[Q73] 查看表状态
来源：http://sjs.jiagoushi.top

SHOW TABLE STATUS LIKE 'users';
来源：http://usd.jqgfzy.top

[Q74] 强制使用索引
来源：http://cvu.hywenlv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nwh.ydzc1.top

[Q75] 日期格式化
来源：http://phi.jqgufenzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://paq.jiagoushi.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bht.fehbvm.com

[Q76] 按天统计
来源：http://mlp.nanxinkj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oln.gogol.net.cn

[Q77] 时间加减
来源：http://xel.gogol.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qae.nwbrower.top

[Q78] 当前时间
来源：http://ywh.chenjidiqi.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tcm.dashuyun.cn

[Q79] 字符串拼接
来源：http://vjs.birdmap.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hab.zdqjudy.top

[Q80] 字符串截取
来源：http://xgh.9152youxi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://axk.tianlin.xyz

[Q81] 字符串替换
来源：http://dfe.nwbrower.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://omu.andypj.xyz

[Q82] 字符长度与字节长度
来源：http://lzu.guannengcc.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nat.ybcxt.top

[Q83] 大小写转换
来源：http://soc.cucudq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ggb.tanke756.top

[Q84] 去除首尾空格
来源：http://vpi.tarul.cn

SELECT TRIM(name) FROM users;
来源：http://trb.hesvh.cn

[Q85] 数值取整
来源：http://eoa.hcnkem.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://clb.hongshengwenyu.top

[Q86] 读取 JSON 字段
来源：http://sbj.yuxming.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xvf.svipenyu.cn

[Q87] JSON 字段做条件
来源：http://wxa.aibaodan.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vhy.vqdsnc.cn

[Q88] 行转列（条件聚合）
来源：http://zma.hfpthk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hny.yj202588.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wzv.zycfv.cn

[Q89] 判断表是否存在
来源：http://oci.gogol.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xuy.zdqjudy.top

[Q90] 生成序号列
来源：http://uay.sweek.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hrj.tarul.cn

================================================================================
来源：http://adj.sysykeji.top

R. Bash 专题
来源：http://xmc.fengsongda.top

================================================================================
来源：http://bmv.ydzc1.top

[R01] shebang 与严格模式
来源：http://lgs.fanxiaobao.xyz

#!/usr/bin/env bash
来源：http://fke.hfpthk.cn

set -euo pipefail
来源：http://xhn.316326.xyz

[R02] 变量赋值与使用
来源：http://qon.hongshengwenyu.top

name="Tom"; echo "$name"
来源：http://ffq.haohaochexian.top

[R03] 只读变量
来源：http://psi.ydzc1.top

readonly PI=3.14
来源：http://usk.zhixingplan.top

[R04] 位置参数
来源：http://dui.pycfn.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://faf.fanxiaobao.xyz

[R05] 参数默认值
来源：http://myw.cucudq.cn

name="${1:-default}"
来源：http://bop.hywenlv.cn

[R06] 判断命令是否存在
来源：http://ree.chenzaomai.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oqy.nanxinkj.top

[R07] if 判断文件
来源：http://wgb.zhaomingkeji.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yrr.redwolf501.top

[R08] 数值比较
来源：http://vzo.hnqzz.top

if (( a > b )); then echo "a 更大"; fi
来源：http://elw.bbcook.cn

[R09] 字符串比较
来源：http://ycf.aizwys.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://njn.chenjidiqi.icu

[R10] 正则匹配
来源：http://yfk.xuetiantiany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wtf.havefunace.top

[R11] case 多分支
来源：http://gzy.52xcode.cn

case "$1" in
来源：http://ezl.sxryk.cn

start) echo "启动" ;;
来源：http://pme.uphjek.com

stop)  echo "停止" ;;
来源：http://jce.guannengcc.top

*)     echo "未知命令" ;;
来源：http://bto.zhiwuduotai.top

esac
来源：http://bzg.birdmap.top

[R12] for 遍历文件
来源：http://ogh.shanyushiyangtech.top

for f in *.txt; do echo "$f"; done
来源：http://bvb.jinqigfzy.top

[R13] for 计数循环
来源：http://mgl.quarkkingdee.top

for i in {1..10}; do echo "$i"; done
来源：http://gky.xziqi.cn

[R14] C 风格 for
来源：http://qpj.kuanghao11.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://glo.xziqi.cn

[R15] while 逐行读文件
来源：http://mlk.zhengqikj.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dwx.guowangkeji.top

[R16] until 等待条件
来源：http://gpn.daria6918.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lju.hywenlv.cn

[R17] 数组定义与取值
来源：http://rgs.mhx1999.top

arr=(a b c); echo "${arr[0]}"
来源：http://vfh.shuidangran.top

[R18] 遍历数组
来源：http://lbf.shzxlz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rzt.ppjwa.cn

[R19] 数组长度
来源：http://div.hnxiangtu.top

echo "${#arr[@]}"
来源：http://nej.pycfn.com

[R20] 关联数组（字典）
来源：http://trh.sxryk.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://buc.yanxiufei.cn

[R21] 字符串长度
来源：http://cik.cdnleiting.top

echo "${#s}"
来源：http://zic.smart0.xyz

[R22] 截取子串
来源：http://khc.zdqjudy.top

echo "${s:0:5}"
来源：http://oph.sjlbkw.cn

[R23] 字符串替换
来源：http://cum.daria6918.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nro.yueranfly.top

[R24] 大小写转换
来源：http://rlp.yj20258.top

echo "${s^^}"; echo "${s,,}"
来源：http://cai.xylfe.cn

[R25] 去后缀 / 去前缀
来源：http://rzb.sxryk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dwf.bjfxy.top

[R26] 命令替换
来源：http://kpf.iojbl.cn

now=$(date +%F); echo "$now"
来源：http://zxm.jiagoushi.top

[R27] 算术展开
来源：http://kzf.chenjidiqi.icu

echo $((1 + 2 * 3))
来源：http://cae.quarkkingdee.top

[R28] 浮点运算
来源：http://jkk.jyoumei.cn

echo "scale=2; 10/3" | bc
来源：http://gey.chenzaomai.com

[R29] 定义函数
来源：http://fya.316326.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pdi.jinqigfzy.top

[R30] 函数返回状态码
来源：http://zuz.c1oappe.top

f() { return 0; }; f || echo "失败了"
来源：http://xfl.zhiwuduotai.top

[R31] 局部变量
来源：http://scz.mhx1999.top

f() { local x=1; echo "$x"; }
来源：http://gur.tanke756.top

[R32] 参数个数校验
来源：http://ffx.tianlin.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xdb.yj20258888.top

[R33] 捕获错误并提示行号
来源：http://qtw.hfpthk.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gwa.ppjwa.cn

[R34] 退出时清理
来源：http://ydx.vehdjk.com

trap 'rm -f "$tmp"' EXIT
来源：http://fcr.hnqzz.top

[R35] 后台执行并等待
来源：http://htf.yuxming.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dml.birdmap.top

[R36] 并发执行多个任务
来源：http://wmr.aibaodan.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ttb.ppjwa.cn

[R37] 把输出赋给变量
来源：http://irr.pengpengdd.cyou

files=$(ls -1)
来源：http://zwu.jinyuanbaomall.cn

[R38] 管道串联
来源：http://myv.hysaishi.cn

cat a.txt | grep -i error | wc -l
来源：http://fxy.hywenlv.cn

[R39] 重定向标准输出与错误
来源：http://mlb.gotoacloud.top

cmd > out.log 2>&1
来源：http://xjv.jinqigufen.top

[R40] 追加写日志
来源：http://ifx.9152youxi.cn

echo "log" >> out.log
来源：http://jav.9152youxi.cn

[R41] 丢弃输出
来源：http://fvn.aizwys.cn

cmd >/dev/null 2>&1
来源：http://igc.sweek.top

[R42] 输入重定向
来源：http://vrw.jyoumei.cn

wc -l < a.txt
来源：http://whn.haohaochexian.top

[R43] 按名字查找文件
来源：http://ihp.dianchejie.cn

find . -name "*.log" -type f
来源：http://ybe.iojbl.cn

[R44] 按修改时间查找
来源：http://oai.nanxinkj.top

find . -mtime -7 -type f
来源：http://cnn.pengpengdd.cyou

[R45] 批量删除
来源：http://tbq.yvedp.cn

find . -name "*.tmp" -delete
来源：http://xdz.uphjek.com

[R46] 递归替换文件内容
来源：http://feg.tianlin.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fxz.0kj1m.cn

[R47] sed 单行替换
来源：http://irq.ydjk.org.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sll.fengsongda.top

[R48] awk 取指定列
来源：http://pic.tianlin.xyz

awk '{print $1, $3}' a.txt
来源：http://dhs.jqgfzy.top

[R49] awk 带条件
来源：http://wfe.yvedp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cld.zdqjudy.top

[R50] awk 求和
来源：http://oya.kuanghao11.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ddq.fzhhl.top

[R51] 排序去重取前几
来源：http://vzi.mhx1999.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jsv.sysykeji.top

[R52] 统计行数
来源：http://kwr.sjlbkw.cn

wc -l a.txt
来源：http://eaf.cheryme.top

[R53] 查看文件头与实时尾
来源：http://zhi.xylfe.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ubt.fehbvm.com

[R54] 比较两个文件
来源：http://hmf.ehwqpu.com

diff a.txt b.txt
来源：http://szw.snrcjt.cn

[R55] 压缩与解压
来源：http://mkk.shanyushiyangtech.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mav.hnqzz.top

[R56] 远程拷贝
来源：http://zej.haohaochexian.top

scp file user@host:/path/
来源：http://fpe.andypj.xyz

[R57] 远程执行命令
来源：http://ysm.birdmap.top

ssh user@host 'uptime'
来源：http://apt.nanxinkj.top

[R58] 下载文件
来源：http://fee.yangfankeji.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gqi.chenjidiqi.icu

[R59] 发 POST JSON
来源：http://gzz.sysykeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://csq.ivvv.top

[R60] 只看 HTTP 状态码
来源：http://rmp.hnxiangtu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kql.zhijiandao.cn

[R61] 磁盘占用
来源：http://gmt.zhoulong.xyz

df -h;  du -sh *
来源：http://iwu.0kj1m.cn

[R62] 找最占空间的文件
来源：http://yan.zycfv.cn

du -ah . | sort -rh | head -10
来源：http://waw.aibaodan.cn

[R63] 内存与进程
来源：http://pet.fehbvm.com

free -h;  ps aux | grep nginx
来源：http://hzl.cdnleiting.top

[R64] 结束进程
来源：http://erq.fanxiaobao.xyz

kill -9 $(pgrep -f app.py)
来源：http://mjs.sufxvd.cn

[R65] 查看端口占用
来源：http://fzh.yangfankeji.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ikv.zhengqikj.top

[R66] 定时任务
来源：http://dyc.zdqjudy.top

crontab -e;  crontab -l
来源：http://rbh.quarkkingdee.top

[R67] 生成随机十六进制串
来源：http://lds.sjlbkw.cn

openssl rand -hex 16
来源：http://pqq.dashuyun.cn

[R68] 计算文件校验值
来源：http://geu.bjfxy.top

sha256sum a.txt;  md5sum a.txt
来源：http://yso.sysykeji.top

[R69] 生成随机密码
来源：http://hua.yueranfly.top

head -c 16 /dev/urandom | base64
来源：http://gvy.feifeiyinyue.top

[R70] 时间戳与互转
来源：http://yjj.daxiang520.top

date +%s;  date -d @1700000000
来源：http://zkt.bbcook.cn

[R71] 日期格式化
来源：http://mfp.bjfxy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lbx.snrcjt.cn

[R72] 等待端口就绪
来源：http://lim.shuidangran.top

until nc -z localhost 3306; do sleep 1; done
来源：http://siy.tarul.cn

[R73] 分割大日志
来源：http://lcp.yonumen.top

split -l 1000 big.log part_
来源：http://ehl.guowangkeji.top

[R74] 批量重命名
来源：http://yjx.sjlbkw.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xkb.redwolf501.top

[R75] 导出环境变量
来源：http://ciw.nanxuanxn.top

export PATH="$HOME/bin:$PATH"
来源：http://vrz.birdmap.top

[R76] 使用临时文件
来源：http://wvd.cqqwz.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rgl.xziqi.cn

[R77] 读取用户输入
来源：http://qgl.chenlongwang.top

read -rp "请输入: " ans
来源：http://ofq.yuanzhike.top

[R78] 交互式菜单
来源：http://ouy.yueranfly.top

select opt in a b c; do echo "$opt"; break; done
来源：http://faz.gotoacloud.top

[R79] 解析命令行选项
来源：http://fff.sysykeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sny.tianlin.xyz

[R80] 查看脚本执行耗时
来源：http://hch.epnwcf.com

time ./run.sh
来源：http://nhp.tian-w.cn

================================================================================
来源：http://wov.yuanzhike.top

S. C / C++ 专题
来源：http://npn.yj20258.top

================================================================================
来源：http://por.yj20258888.top

[S01] C：Hello World
来源：http://dqp.wangdashe.top

#include <stdio.h>
来源：http://plt.ivvv.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://uao.chenzaomai.com

[S02] C：变量与格式化输出
来源：http://its.xinyue.icu

int a = 10; printf("%d\n", a);
来源：http://gai.xingfuxueyuan.xyz

[S03] C：读入整数
来源：http://rpm.pengpengdd.cyou

int x; scanf("%d", &x);
来源：http://kpy.hongshengwenyu.top

[S04] C：字符串复制
来源：http://uql.guannengcc.top

char dst[32]; strcpy(dst, "hi");
来源：http://bun.cucudq.cn

[S05] C：字符串长度
来源：http://jgr.havefunace.top

strlen(s)
来源：http://lte.cheryme.top

[S06] C：字符串比较
来源：http://ujj.jlsjyb.cn

strcmp(a, b) == 0
来源：http://uuw.sjlbkw.cn

[S07] C：数组遍历求和
来源：http://ixo.ehwqpu.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xdd.hywenlv.cn

[S08] C：动态内存分配与释放
来源：http://gpj.kuanghao11.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xfn.aizwys.cn

[S09] C：结构体定义与初始化
来源：http://xyo.316326.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ajd.hcnkem.com

[S10] C：指针与解引用
来源：http://zxs.cdnleiting.top

int *p = &a;  *p = 5;
来源：http://vyo.quarkkingdee.top

[S11] C：逐行读文件
来源：http://phw.gogol.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://dlb.fanxiaobao.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://puy.jinqigfzy.top

fclose(f);
来源：http://chv.tianlin.xyz

[S12] C：写文件
来源：http://kbr.sufxvd.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zmd.wangdashe.top

[S13] C：宏定义
来源：http://chm.tarul.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mik.0kj1m.cn

[S14] C：枚举
来源：http://mfl.shangyingyoupin.top

enum Color { RED, GREEN, BLUE };
来源：http://uvm.hnqzz.top

[S15] C：类型转换
来源：http://xww.aizwys.cn

(double) a / b
来源：http://nwr.zhongyouzk.top

[S16] C：位操作置位
来源：http://gcg.birdmap.top

x |= (1 << 3);
来源：http://gfq.ctjpmb.com

[S17] C：安全拼接字符串
来源：http://njh.yueranfly.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wsn.jinyuanbaomall.cn

[S18] C：命令行参数
来源：http://cju.xziqi.cn

int main(int argc, char **argv)
来源：http://tbn.aizwys.cn

[S19] C：快速排序
来源：http://mxe.ywan-chungtsiang.top

qsort(a, n, sizeof(int), cmp);
来源：http://aqm.ivvv.top

[S20] C：二分查找
来源：http://zlc.c1oappe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dze.nwbrower.top

[S21] C：字符类别判断
来源：http://xdy.chenjidiqi.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kgi.pycfn.com

[S22] C：字符串转数字
来源：http://bzr.feifeiyinyue.top

atoi("42");  strtod("3.14", NULL);
来源：http://pee.hcnkem.com

[S23] C：随机数
来源：http://fqk.chenzaomai.com

srand(time(NULL));  int r = rand() % 100;
来源：http://lhi.quarkkingdee.top

[S24] C：获取本地时间
来源：http://vrw.yj20258.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sen.birdmap.top

[S25] C：内存拷贝
来源：http://pjx.xuetiantiany.cn

memcpy(dst, src, n);
来源：http://ohb.zhixingplan.top

[S26] C：内存清零
来源：http://bif.zhongyouzk.top

memset(a, 0, sizeof a);
来源：http://lvm.xziqi.cn

[S27] C：定义常量
来源：http://hpj.xuetiantiany.cn

const double PI = 3.14159;
来源：http://cqf.mhx1999.top

[S28] C：静态变量
来源：http://agu.hesvh.cn

static int counter = 0;
来源：http://kpy.daxiang520.top

[S29] C：变参函数
来源：http://csm.wangshuangyany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dlo.bbcook.cn

[S30] C：头文件保护
来源：http://isl.aibaodan.cn

#ifndef X_H
来源：http://zyk.snrcjt.cn

#define X_H
来源：http://exs.pengpengdd.cyou

#endif
来源：http://toy.cheryme.top

[S31] C++：Hello World
来源：http://liu.yvedp.cn

#include <iostream>
来源：http://dkc.yangfankeji.com

int main() { std::cout << "Hello\n"; }
来源：http://sbk.uphjek.com

[S32] C++：字符串
来源：http://qvf.cheryme.top

std::string s = "hi";  s += "!";
来源：http://yjz.hnqzz.top

[S33] C++：vector 增删
来源：http://hfj.ybcxt.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pmx.haohaochexian.top

[S34] C++：遍历 vector
来源：http://spj.ydjk.org.cn

for (auto &x : v) { std::cout << x; }
来源：http://aot.iojbl.cn

[S35] C++：map
来源：http://lcn.cqqwz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kov.tanke756.top

[S36] C++：unordered_map
来源：http://asc.kuanghao11.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qkc.gotoacloud.top

[S37] C++：set
来源：http://pfz.tianlin.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hom.iojbl.cn

[S38] C++：排序
来源：http://fpc.daria6918.cn

std::sort(v.begin(), v.end());
来源：http://fiy.gogol.net.cn


<!-- 参考信息 -->