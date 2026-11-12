代发 wailian999

[Q63] 开启事务
来源：http://lnz.zhixingplan.top

START TRANSACTION;                -- 或 BEGIN
来源：http://edz.hnqzz.top

[Q64] 提交事务
来源：http://qrc.nanxuanxn.top

COMMIT;
来源：http://xis.bbcook.cn

[Q65] 回滚事务
来源：http://epm.sufxvd.cn

ROLLBACK;
来源：http://toe.hysaishi.cn

[Q66] 行锁查询
来源：http://msi.xingfuxueyuan.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://phc.sysykeji.top

[Q67] 设置隔离级别
来源：http://kma.sjlbkw.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ltd.jlsjyb.cn

[Q68] 保存点
来源：http://twx.yonumen.top

SAVEPOINT sp1;
来源：http://pgs.nanxinkj.top

ROLLBACK TO sp1;
来源：http://pou.fktsv.cn

[Q69] 查看执行计划
来源：http://yjl.smart0.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://iuu.zhijiandao.cn

[Q70] 更新统计信息
来源：http://bif.aibaodan.cn

ANALYZE TABLE users;
来源：http://apl.cucudq.cn

[Q71] 查看建表语句
来源：http://uwy.sweek.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nui.yvedp.cn

[Q72] 查看索引
来源：http://gfj.hammf.cn

SHOW INDEX FROM users;
来源：http://iij.cdnleiting.top

[Q73] 查看表状态
来源：http://kmb.gzhubu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://lby.jinghuilouyu.cn

[Q74] 强制使用索引
来源：http://ehp.svipenyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://muj.jqgufenzy.top

[Q75] 日期格式化
来源：http://ego.tian-w.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ssv.c1oappe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eyq.jinghuilouyu.cn

[Q76] 按天统计
来源：http://dsu.nanxuanxn.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sel.yanxiufei.cn

[Q77] 时间加减
来源：http://duv.52xcode.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tca.andypj.xyz

[Q78] 当前时间
来源：http://sxq.fanxiaobao.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://stb.guowangkeji.top

[Q79] 字符串拼接
来源：http://tun.quarkkingdee.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tcv.cashguo.top

[Q80] 字符串截取
来源：http://mzh.tianlin.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://omb.zdqjudy.top

[Q81] 字符串替换
来源：http://gqp.yuanzhike.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cwl.daria6918.cn

[Q82] 字符长度与字节长度
来源：http://eyb.andypj.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hbv.birdmap.top

[Q83] 大小写转换
来源：http://fbv.kuanghao11.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zly.epnwcf.com

[Q84] 去除首尾空格
来源：http://lhp.xuanzx.com

SELECT TRIM(name) FROM users;
来源：http://hks.hesvh.cn

[Q85] 数值取整
来源：http://kan.jianghu66.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://klb.sysykeji.top

[Q86] 读取 JSON 字段
来源：http://owp.jqgufenzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ajf.epnwcf.com

[Q87] JSON 字段做条件
来源：http://atr.jianghu66.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qxj.hammf.cn

[Q88] 行转列（条件聚合）
来源：http://van.xuetiantiany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cbp.yueranfly.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://trz.fanxiaobao.xyz

[Q89] 判断表是否存在
来源：http://ocf.dashuyun.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xis.hywenlv.cn

[Q90] 生成序号列
来源：http://rij.ctjpmb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kih.zdbjq.cn

================================================================================
来源：http://xqs.zycfv.cn

R. Bash 专题
来源：http://azx.ehwqpu.com

================================================================================
来源：http://fzk.hywenlv.cn

[R01] shebang 与严格模式
来源：http://wvc.guowangkeji.top

#!/usr/bin/env bash
来源：http://jrq.hfpthk.cn

set -euo pipefail
来源：http://ldz.tian-w.cn

[R02] 变量赋值与使用
来源：http://mzp.yfazqb.com

name="Tom"; echo "$name"
来源：http://ikt.cqqwz.cn

[R03] 只读变量
来源：http://nuv.c1oappe.top

readonly PI=3.14
来源：http://kkz.ctjpmb.com

[R04] 位置参数
来源：http://weh.hysaishi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ccj.shzxlz.cn

[R05] 参数默认值
来源：http://eov.cdnleiting.top

name="${1:-default}"
来源：http://huz.52xcode.cn

[R06] 判断命令是否存在
来源：http://rqt.redwolf501.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tfz.tanke756.top

[R07] if 判断文件
来源：http://lqx.zhaomingkeji.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wss.pycfn.com

[R08] 数值比较
来源：http://pay.jqgfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ynh.zhengqikj.top

[R09] 字符串比较
来源：http://nxp.zhengqikj.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://irw.hnqzz.top

[R10] 正则匹配
来源：http://cdb.hcnkem.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jeu.jiagoushi.top

[R11] case 多分支
来源：http://xoy.tarul.cn

case "$1" in
来源：http://zsa.wangdashe.top

start) echo "启动" ;;
来源：http://gqd.zhoulong.xyz

stop)  echo "停止" ;;
来源：http://ccc.ehwqpu.com

*)     echo "未知命令" ;;
来源：http://yry.jianghu66.top

esac
来源：http://iag.jinghuilouyu.cn

[R12] for 遍历文件
来源：http://swj.sxryk.cn

for f in *.txt; do echo "$f"; done
来源：http://cpq.hcnkem.com

[R13] for 计数循环
来源：http://vff.bjfxy.top

for i in {1..10}; do echo "$i"; done
来源：http://vrd.sysykeji.top

[R14] C 风格 for
来源：http://ymf.yj20258.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dyc.zhongyouzk.top

[R15] while 逐行读文件
来源：http://xug.wangshuangyany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wqp.yj20258888.top

[R16] until 等待条件
来源：http://ypx.hcnkem.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mlo.jinqigfzy.top

[R17] 数组定义与取值
来源：http://wvy.zdqjudy.top

arr=(a b c); echo "${arr[0]}"
来源：http://pyx.sufxvd.cn

[R18] 遍历数组
来源：http://eyk.nanxinkj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kgg.jinqigufen.top

[R19] 数组长度
来源：http://une.hfpthk.cn

echo "${#arr[@]}"
来源：http://hvj.uphjek.com

[R20] 关联数组（字典）
来源：http://ksl.chenjidiqi.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fof.aibaodan.cn

[R21] 字符串长度
来源：http://qeh.svipenyu.cn

echo "${#s}"
来源：http://kju.jinqigufen.top

[R22] 截取子串
来源：http://rfw.jinghuilouyu.cn

echo "${s:0:5}"
来源：http://axn.cashguo.top

[R23] 字符串替换
来源：http://jmp.tanke756.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://opq.yueranfly.top

[R24] 大小写转换
来源：http://hqm.zhixingplan.top

echo "${s^^}"; echo "${s,,}"
来源：http://afh.wangdashe.top

[R25] 去后缀 / 去前缀
来源：http://avq.yuxming.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fhj.bjfxy.top

[R26] 命令替换
来源：http://wvw.ydjk.org.cn

now=$(date +%F); echo "$now"
来源：http://xjz.ydzc1.top

[R27] 算术展开
来源：http://pjk.dashuyun.cn

echo $((1 + 2 * 3))
来源：http://lxt.ehwqpu.com

[R28] 浮点运算
来源：http://mjx.chenzaomai.com

echo "scale=2; 10/3" | bc
来源：http://pff.52xcode.cn

[R29] 定义函数
来源：http://spl.sweek.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rra.c1oappe.top

[R30] 函数返回状态码
来源：http://yvc.ivvv.top

f() { return 0; }; f || echo "失败了"
来源：http://oxk.xuetiantiany.cn

[R31] 局部变量
来源：http://eau.yanxiufei.cn

f() { local x=1; echo "$x"; }
来源：http://kli.sufxvd.cn

[R32] 参数个数校验
来源：http://hfq.52xcode.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wpj.daria6918.cn

[R33] 捕获错误并提示行号
来源：http://bvc.zhongyouzk.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tru.jinghuilouyu.cn

[R34] 退出时清理
来源：http://rby.yfazqb.com

trap 'rm -f "$tmp"' EXIT
来源：http://ifd.cqqwz.cn

[R35] 后台执行并等待
来源：http://yyo.gaohongyu789.top

sleep 5 & pid=$!; wait "$pid"
来源：http://oyt.sxryk.cn

[R36] 并发执行多个任务
来源：http://ujx.tianlin.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iof.quarkkingdee.top

[R37] 把输出赋给变量
来源：http://wev.ydjk.org.cn

files=$(ls -1)
来源：http://ulm.shuidangran.top

[R38] 管道串联
来源：http://cpc.shzxlz.cn

cat a.txt | grep -i error | wc -l
来源：http://dtu.gzhubu.top

[R39] 重定向标准输出与错误
来源：http://rfg.ppjwa.cn

cmd > out.log 2>&1
来源：http://xae.dashuyun.cn

[R40] 追加写日志
来源：http://xjc.shzxlz.cn

echo "log" >> out.log
来源：http://feo.hfpthk.cn

[R41] 丢弃输出
来源：http://cda.xuanzx.com

cmd >/dev/null 2>&1
来源：http://rev.snrcjt.cn

[R42] 输入重定向
来源：http://bat.chenlongwang.top

wc -l < a.txt
来源：http://wej.shanyushiyangtech.top

[R43] 按名字查找文件
来源：http://gcv.gaohongyu789.top

find . -name "*.log" -type f
来源：http://xda.tian-w.cn

[R44] 按修改时间查找
来源：http://ygl.sjlbkw.cn

find . -mtime -7 -type f
来源：http://emt.wangdashe.top

[R45] 批量删除
来源：http://efy.yueranfly.top

find . -name "*.tmp" -delete
来源：http://ndg.c1oappe.top

[R46] 递归替换文件内容
来源：http://nam.yvedp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xxj.zycfv.cn

[R47] sed 单行替换
来源：http://smj.zhoulong.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://cyw.shuidangran.top

[R48] awk 取指定列
来源：http://avg.ivvv.top

awk '{print $1, $3}' a.txt
来源：http://xoq.iojbl.cn

[R49] awk 带条件
来源：http://rwz.yueranfly.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mdc.tian-w.cn

[R50] awk 求和
来源：http://qgp.cheryme.top

awk '{s += $2} END {print s}' a.txt
来源：http://ciu.dianchejie.cn

[R51] 排序去重取前几
来源：http://jbt.cucudq.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zwi.nanxinkj.top

[R52] 统计行数
来源：http://jpq.yfazqb.com

wc -l a.txt
来源：http://fpc.bbcook.cn

[R53] 查看文件头与实时尾
来源：http://jki.jinqigufen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ltz.sufxvd.cn

[R54] 比较两个文件
来源：http://uup.sweek.top

diff a.txt b.txt
来源：http://pta.nanxuanxn.top

[R55] 压缩与解压
来源：http://gmk.redwolf501.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zsb.jqgfzy.top

[R56] 远程拷贝
来源：http://kbf.hnxiangtu.top

scp file user@host:/path/
来源：http://urt.cdnleiting.top

[R57] 远程执行命令
来源：http://uih.yuxming.cn

ssh user@host 'uptime'
来源：http://suu.aibaodan.cn

[R58] 下载文件
来源：http://ppf.fzhhl.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://axb.tarul.cn

[R59] 发 POST JSON
来源：http://gaw.hywenlv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xjf.mhx1999.top

[R60] 只看 HTTP 状态码
来源：http://rhq.jinyuanbaomall.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://abx.mhx1999.top

[R61] 磁盘占用
来源：http://bfp.svipenyu.cn

df -h;  du -sh *
来源：http://ntn.guannengcc.top

[R62] 找最占空间的文件
来源：http://wsy.jqgfzy.top

du -ah . | sort -rh | head -10
来源：http://loy.jlsjyb.cn

[R63] 内存与进程
来源：http://hac.jinqigufen.top

free -h;  ps aux | grep nginx
来源：http://zbe.yj20258.top

[R64] 结束进程
来源：http://ctk.yongpay.top

kill -9 $(pgrep -f app.py)
来源：http://rkd.svipenyu.cn

[R65] 查看端口占用
来源：http://ngk.xylfe.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dia.quarkkingdee.top

[R66] 定时任务
来源：http://lqm.zdqjudy.top

crontab -e;  crontab -l
来源：http://ruk.ywan-chungtsiang.top

[R67] 生成随机十六进制串
来源：http://dmt.ctjpmb.com

openssl rand -hex 16
来源：http://bim.xingfuxueyuan.xyz

[R68] 计算文件校验值
来源：http://dum.zhiwuduotai.top

sha256sum a.txt;  md5sum a.txt
来源：http://gsx.jinyuanbaomall.cn

[R69] 生成随机密码
来源：http://xqe.nwbrower.top

head -c 16 /dev/urandom | base64
来源：http://qxj.hfpthk.cn

[R70] 时间戳与互转
来源：http://sba.aizwys.cn

date +%s;  date -d @1700000000
来源：http://njk.jinqigfzy.top

[R71] 日期格式化
来源：http://nyq.shanyushiyangkeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ifz.daxiang520.top

[R72] 等待端口就绪
来源：http://xty.daria6918.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hcv.smart0.xyz

[R73] 分割大日志
来源：http://zxx.zhongyouzk.top

split -l 1000 big.log part_
来源：http://dce.sweek.top

[R74] 批量重命名
来源：http://nvz.redwolf501.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fdy.jiagoushi.top

[R75] 导出环境变量
来源：http://yls.vehdjk.com

export PATH="$HOME/bin:$PATH"
来源：http://cdp.fehbvm.com

[R76] 使用临时文件
来源：http://dqc.sufxvd.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hvm.sysykeji.top

[R77] 读取用户输入
来源：http://tmm.nanxuanxn.top

read -rp "请输入: " ans
来源：http://mkj.ywan-chungtsiang.top

[R78] 交互式菜单
来源：http://dnt.jqgufenzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://fow.xuanzx.com

[R79] 解析命令行选项
来源：http://jov.ydjk.org.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xoj.xingfuxueyuan.xyz

[R80] 查看脚本执行耗时
来源：http://obo.cdnleiting.top

time ./run.sh
来源：http://rmg.nwbrower.top

================================================================================
来源：http://cvm.vehdjk.com

S. C / C++ 专题
来源：http://lva.yj20258888.top

================================================================================
来源：http://snk.ppjwa.cn

[S01] C：Hello World
来源：http://ciz.xziqi.cn

#include <stdio.h>
来源：http://gft.ywan-chungtsiang.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wsu.jinqigufen.top

[S02] C：变量与格式化输出
来源：http://fsv.ppjwa.cn

int a = 10; printf("%d\n", a);
来源：http://xlo.birdmap.top

[S03] C：读入整数
来源：http://czx.fktsv.cn

int x; scanf("%d", &x);
来源：http://omv.yangfankeji.com

[S04] C：字符串复制
来源：http://swo.sjlbkw.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zfu.mhx1999.top

[S05] C：字符串长度
来源：http://mks.chenlongwang.top

strlen(s)
来源：http://cks.quarkkingdee.top

[S06] C：字符串比较
来源：http://tsi.ydzc1.top

strcmp(a, b) == 0
来源：http://hmp.dianchejie.cn

[S07] C：数组遍历求和
来源：http://xdv.jinghuilouyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ynh.tian-w.cn

[S08] C：动态内存分配与释放
来源：http://qql.yj202588.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rkw.0kj1m.cn

[S09] C：结构体定义与初始化
来源：http://usv.c1oappe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qbl.xinyue.icu

[S10] C：指针与解引用
来源：http://rzg.cdnleiting.top

int *p = &a;  *p = 5;
来源：http://lbk.dianchejie.cn

[S11] C：逐行读文件
来源：http://hcp.cheryme.top

FILE *f = fopen("a.txt", "r");
来源：http://wev.xinyue.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://kei.vehdjk.com

fclose(f);
来源：http://myy.hammf.cn

[S12] C：写文件
来源：http://eii.ybcxt.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ost.xziqi.cn

[S13] C：宏定义
来源：http://cet.redwolf501.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ccm.zhengqikj.top

[S14] C：枚举
来源：http://zcf.jyoumei.cn

enum Color { RED, GREEN, BLUE };
来源：http://hym.pycfn.com

[S15] C：类型转换
来源：http://eyj.shuidangran.top

(double) a / b
来源：http://dkn.fehbvm.com

[S16] C：位操作置位
来源：http://mhl.cucudq.cn

x |= (1 << 3);
来源：http://yhq.smart0.xyz

[S17] C：安全拼接字符串
来源：http://err.yj20258.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nwv.sxryk.cn

[S18] C：命令行参数
来源：http://akj.cucudq.cn

int main(int argc, char **argv)
来源：http://jjf.hammf.cn

[S19] C：快速排序
来源：http://bck.haohaochexian.top

qsort(a, n, sizeof(int), cmp);
来源：http://bnk.zdqjudy.top

[S20] C：二分查找
来源：http://rek.xinyue.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fyc.yj20258.top

[S21] C：字符类别判断
来源：http://dsr.gogol.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://leg.jqgufenzy.top

[S22] C：字符串转数字
来源：http://ksc.ybcxt.top

atoi("42");  strtod("3.14", NULL);
来源：http://cao.hnqzz.top

[S23] C：随机数
来源：http://xql.sweek.top

srand(time(NULL));  int r = rand() % 100;
来源：http://uim.zdbjq.cn

[S24] C：获取本地时间
来源：http://tsa.hesvh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yxi.zdbjq.cn

[S25] C：内存拷贝
来源：http://qrx.xinyue.icu

memcpy(dst, src, n);
来源：http://ynt.jiagoushi.top

[S26] C：内存清零
来源：http://ueb.yangfankeji.com

memset(a, 0, sizeof a);
来源：http://ztf.fehbvm.com

[S27] C：定义常量
来源：http://zgu.ywan-chungtsiang.top

const double PI = 3.14159;
来源：http://kjt.uphjek.com

[S28] C：静态变量
来源：http://vxz.hcnkem.com

static int counter = 0;
来源：http://cgt.fzhhl.top

[S29] C：变参函数
来源：http://odl.andypj.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bxt.cqqwz.cn

[S30] C：头文件保护
来源：http://dly.shanyushiyangtech.top

#ifndef X_H
来源：http://ofz.zhixingplan.top

#define X_H
来源：http://wpv.shanyushiyangkeji.top

#endif
来源：http://xir.sjlbkw.cn

[S31] C++：Hello World
来源：http://pwa.yvedp.cn

#include <iostream>
来源：http://wbj.zhiwuduotai.top

int main() { std::cout << "Hello\n"; }
来源：http://wdc.ctjpmb.com

[S32] C++：字符串
来源：http://jaj.xinyue.icu

std::string s = "hi";  s += "!";
来源：http://wci.vqdsnc.cn


<!-- 参考信息 -->