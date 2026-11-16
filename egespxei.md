代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hrb.fktsv.cn

[Q58] 累计求和
来源：http://azq.bjfxy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sbx.shuidangran.top

[Q59] 分组内累计
来源：http://eol.epnwcf.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rrl.ctjpmb.com

[Q60] 取上一行 / 下一行
来源：http://xzm.xinyue.icu

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nxi.xuanzx.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xlp.xylfe.cn

[Q61] 移动平均
来源：http://wzd.snrcjt.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lez.zycfv.cn

[Q62] 分组占比
来源：http://gtp.fengsongda.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hhg.tanke756.top

[Q63] 开启事务
来源：http://mlh.ivvv.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wtn.hongshengwenyu.top

[Q64] 提交事务
来源：http://xqm.smart0.xyz

COMMIT;
来源：http://sow.hesvh.cn

[Q65] 回滚事务
来源：http://dzn.sweek.top

ROLLBACK;
来源：http://nqz.cqqwz.cn

[Q66] 行锁查询
来源：http://aul.dianchejie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://myc.shuidangran.top

[Q67] 设置隔离级别
来源：http://zzq.zdqjudy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rez.hywenlv.cn

[Q68] 保存点
来源：http://nei.jinghuilouyu.cn

SAVEPOINT sp1;
来源：http://vba.shangyingyoupin.top

ROLLBACK TO sp1;
来源：http://wbp.xylfe.cn

[Q69] 查看执行计划
来源：http://kqj.jianghu66.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xbe.quarkkingdee.top

[Q70] 更新统计信息
来源：http://zqm.sweek.top

ANALYZE TABLE users;
来源：http://dni.zhaomingkeji.xyz

[Q71] 查看建表语句
来源：http://kpb.meibo888.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jge.ctjpmb.com

[Q72] 查看索引
来源：http://mbv.zhijiandao.cn

SHOW INDEX FROM users;
来源：http://rei.52xcode.cn

[Q73] 查看表状态
来源：http://qvz.shanyushiyangtech.top

SHOW TABLE STATUS LIKE 'users';
来源：http://muj.sufxvd.cn

[Q74] 强制使用索引
来源：http://edk.smart0.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nsi.yj20258888.top

[Q75] 日期格式化
来源：http://xqq.fanxiaobao.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xgq.ppjwa.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tar.jinyuanbaomall.cn

[Q76] 按天统计
来源：http://cur.hongshengwenyu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dzv.birdmap.top

[Q77] 时间加减
来源：http://vrz.ydjk.org.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://stk.jinyuanbaomall.cn

[Q78] 当前时间
来源：http://hgj.9152youxi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yrt.pengpengdd.cyou

[Q79] 字符串拼接
来源：http://ehg.vqdsnc.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ehb.chenzaomai.com

[Q80] 字符串截取
来源：http://dmc.pycfn.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://poz.guowangkeji.top

[Q81] 字符串替换
来源：http://drr.nanxuanxn.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xcg.yueranfly.top

[Q82] 字符长度与字节长度
来源：http://jja.tanke756.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://iyh.mhx1999.top

[Q83] 大小写转换
来源：http://dsb.c1oappe.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lgj.pycfn.com

[Q84] 去除首尾空格
来源：http://xrp.feifeiyinyue.top

SELECT TRIM(name) FROM users;
来源：http://loa.ppjwa.cn

[Q85] 数值取整
来源：http://xyw.dianchejie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rdy.ctjpmb.com

[Q86] 读取 JSON 字段
来源：http://aft.nanxinkj.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://feq.quarkkingdee.top

[Q87] JSON 字段做条件
来源：http://tji.zdqjudy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sfn.jianghu66.top

[Q88] 行转列（条件聚合）
来源：http://gfw.cucudq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cnt.bjfxy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zbc.wangshuangyany.cn

[Q89] 判断表是否存在
来源：http://itg.yueranfly.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://aob.shanyushiyangkeji.top

[Q90] 生成序号列
来源：http://tvb.jlsjyb.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rdg.wangdashe.top

================================================================================
来源：http://mes.yanxiufei.cn

R. Bash 专题
来源：http://aqo.ydzc1.top

================================================================================
来源：http://lco.cucudq.cn

[R01] shebang 与严格模式
来源：http://edi.andypj.xyz

#!/usr/bin/env bash
来源：http://nqv.sxryk.cn

set -euo pipefail
来源：http://fxj.tanke756.top

[R02] 变量赋值与使用
来源：http://wbi.zdbjq.cn

name="Tom"; echo "$name"
来源：http://wcm.hammf.cn

[R03] 只读变量
来源：http://tqj.yangfankeji.com

readonly PI=3.14
来源：http://mrh.sufxvd.cn

[R04] 位置参数
来源：http://owb.zhengqikj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://htk.hysaishi.cn

[R05] 参数默认值
来源：http://mvi.jinqigfzy.top

name="${1:-default}"
来源：http://jtg.cheryme.top

[R06] 判断命令是否存在
来源：http://pck.zdqjudy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xwq.daria6918.cn

[R07] if 判断文件
来源：http://uaq.yangfankeji.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://inh.xuetiantiany.cn

[R08] 数值比较
来源：http://uhv.dashuyun.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://aqk.uphjek.com

[R09] 字符串比较
来源：http://adn.52xcode.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ugu.bjfxy.top

[R10] 正则匹配
来源：http://ghh.mhx1999.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pky.jinqigfzy.top

[R11] case 多分支
来源：http://dpk.yj20258.top

case "$1" in
来源：http://ola.ppjwa.cn

start) echo "启动" ;;
来源：http://tdd.ybcxt.top

stop)  echo "停止" ;;
来源：http://abx.zhongyouzk.top

*)     echo "未知命令" ;;
来源：http://fof.zhaomingkeji.xyz

esac
来源：http://bgz.iojbl.cn

[R12] for 遍历文件
来源：http://ptb.tarul.cn

for f in *.txt; do echo "$f"; done
来源：http://tcg.iojbl.cn

[R13] for 计数循环
来源：http://sni.daxiang520.top

for i in {1..10}; do echo "$i"; done
来源：http://cvr.tanke756.top

[R14] C 风格 for
来源：http://ezk.hfpthk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cbs.tianlin.xyz

[R15] while 逐行读文件
来源：http://fbr.shzxlz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uhq.chenlongwang.top

[R16] until 等待条件
来源：http://jos.ppjwa.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zar.shzxlz.cn

[R17] 数组定义与取值
来源：http://olw.zhixingplan.top

arr=(a b c); echo "${arr[0]}"
来源：http://ofe.cheryme.top

[R18] 遍历数组
来源：http://uon.sjlbkw.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rdb.fzhhl.top

[R19] 数组长度
来源：http://fua.shanyushiyangkeji.top

echo "${#arr[@]}"
来源：http://rns.yanxiufei.cn

[R20] 关联数组（字典）
来源：http://faq.316326.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dcd.cheryme.top

[R21] 字符串长度
来源：http://nfz.ehwqpu.com

echo "${#s}"
来源：http://ksc.shanyushiyangtech.top

[R22] 截取子串
来源：http://avs.hesvh.cn

echo "${s:0:5}"
来源：http://lfa.sxryk.cn

[R23] 字符串替换
来源：http://ipu.zhiwuduotai.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tcy.gaohongyu789.top

[R24] 大小写转换
来源：http://jjj.havefunace.top

echo "${s^^}"; echo "${s,,}"
来源：http://brj.zhengqikj.top

[R25] 去后缀 / 去前缀
来源：http://zzz.feifeiyinyue.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mey.cqqwz.cn

[R26] 命令替换
来源：http://mvy.kuanghao11.cn

now=$(date +%F); echo "$now"
来源：http://yml.svipenyu.cn

[R27] 算术展开
来源：http://ljl.vehdjk.com

echo $((1 + 2 * 3))
来源：http://eax.cashguo.top

[R28] 浮点运算
来源：http://faq.chenzaomai.com

echo "scale=2; 10/3" | bc
来源：http://ftn.ivvv.top

[R29] 定义函数
来源：http://mrs.zdbjq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://szt.guowangkeji.top

[R30] 函数返回状态码
来源：http://jnr.xylfe.cn

f() { return 0; }; f || echo "失败了"
来源：http://qhu.hywenlv.cn

[R31] 局部变量
来源：http://tdq.feifeiyinyue.top

f() { local x=1; echo "$x"; }
来源：http://upj.shanyushiyangkeji.top

[R32] 参数个数校验
来源：http://ede.shzxlz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jms.xuanzx.com

[R33] 捕获错误并提示行号
来源：http://xge.pengpengdd.cyou

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yyf.jlsjyb.cn

[R34] 退出时清理
来源：http://mhx.xuetiantiany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rrt.shangyingyoupin.top

[R35] 后台执行并等待
来源：http://ina.jlsjyb.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cvx.zdbjq.cn

[R36] 并发执行多个任务
来源：http://isl.yanxiufei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vbq.yuanzhike.top

[R37] 把输出赋给变量
来源：http://ujn.xinyue.icu

files=$(ls -1)
来源：http://mmv.shangyingyoupin.top

[R38] 管道串联
来源：http://kqz.meibo888.top

cat a.txt | grep -i error | wc -l
来源：http://isg.zdbjq.cn

[R39] 重定向标准输出与错误
来源：http://ajs.shzxlz.cn

cmd > out.log 2>&1
来源：http://kww.aizwys.cn

[R40] 追加写日志
来源：http://kuo.yuxming.cn

echo "log" >> out.log
来源：http://jdp.andypj.xyz

[R41] 丢弃输出
来源：http://arb.gaohongyu789.top

cmd >/dev/null 2>&1
来源：http://mdy.ybcxt.top

[R42] 输入重定向
来源：http://zqe.sxryk.cn

wc -l < a.txt
来源：http://sbt.tanke756.top

[R43] 按名字查找文件
来源：http://eqd.daria6918.cn

find . -name "*.log" -type f
来源：http://lcp.yonumen.top

[R44] 按修改时间查找
来源：http://mul.zhoulong.xyz

find . -mtime -7 -type f
来源：http://hrp.epnwcf.com

[R45] 批量删除
来源：http://jhf.hcnkem.com

find . -name "*.tmp" -delete
来源：http://aww.ppjwa.cn

[R46] 递归替换文件内容
来源：http://iup.hfpthk.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kjv.fktsv.cn

[R47] sed 单行替换
来源：http://uht.fehbvm.com

sed -i 's/foo/bar/g' a.txt
来源：http://hog.fanxiaobao.xyz

[R48] awk 取指定列
来源：http://lem.epnwcf.com

awk '{print $1, $3}' a.txt
来源：http://vgz.ivvv.top

[R49] awk 带条件
来源：http://gdk.jqgufenzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dgo.gotoacloud.top

[R50] awk 求和
来源：http://gch.shanyushiyangtech.top

awk '{s += $2} END {print s}' a.txt
来源：http://ivj.shuidangran.top

[R51] 排序去重取前几
来源：http://htr.sxryk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zub.ywan-chungtsiang.top

[R52] 统计行数
来源：http://ffc.hnxiangtu.top

wc -l a.txt
来源：http://gvn.zdbjq.cn

[R53] 查看文件头与实时尾
来源：http://kam.dashuyun.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oio.zhengqikj.top

[R54] 比较两个文件
来源：http://gux.chenlongwang.top

diff a.txt b.txt
来源：http://dcn.wangdashe.top

[R55] 压缩与解压
来源：http://iat.hesvh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://icn.chenjidiqi.icu

[R56] 远程拷贝
来源：http://ujp.ivvv.top

scp file user@host:/path/
来源：http://num.jianghu66.top

[R57] 远程执行命令
来源：http://zbo.jqgfzy.top

ssh user@host 'uptime'
来源：http://phy.sxryk.cn

[R58] 下载文件
来源：http://yze.fktsv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pym.yj20258.top

[R59] 发 POST JSON
来源：http://wac.daxiang520.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mxb.shangyingyoupin.top

[R60] 只看 HTTP 状态码
来源：http://rba.zhoulong.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ocn.vehdjk.com

[R61] 磁盘占用
来源：http://uoj.hywenlv.cn

df -h;  du -sh *
来源：http://wle.zhengqikj.top

[R62] 找最占空间的文件
来源：http://msg.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://amj.smart0.xyz

[R63] 内存与进程
来源：http://kob.mhx1999.top

free -h;  ps aux | grep nginx
来源：http://raq.gotoacloud.top

[R64] 结束进程
来源：http://ycv.cashguo.top

kill -9 $(pgrep -f app.py)
来源：http://hfo.tian-w.cn

[R65] 查看端口占用
来源：http://zyr.xinyue.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hoq.gzhubu.top

[R66] 定时任务
来源：http://iir.hnxiangtu.top

crontab -e;  crontab -l
来源：http://scy.snrcjt.cn

[R67] 生成随机十六进制串
来源：http://wrf.xingfuxueyuan.xyz

openssl rand -hex 16
来源：http://gtk.sweek.top

[R68] 计算文件校验值
来源：http://twr.ppjwa.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vsb.xziqi.cn

[R69] 生成随机密码
来源：http://nlg.ywan-chungtsiang.top

head -c 16 /dev/urandom | base64
来源：http://fau.svipenyu.cn

[R70] 时间戳与互转
来源：http://ezs.bjfxy.top

date +%s;  date -d @1700000000
来源：http://ria.guowangkeji.top

[R71] 日期格式化
来源：http://dos.yj20258888.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://hus.hcnkem.com

[R72] 等待端口就绪
来源：http://whc.shuidangran.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mji.zhengqikj.top

[R73] 分割大日志
来源：http://duu.fzhhl.top

split -l 1000 big.log part_
来源：http://vgj.tarul.cn

[R74] 批量重命名
来源：http://rum.zhiwuduotai.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nrr.sxryk.cn

[R75] 导出环境变量
来源：http://qob.guannengcc.top

export PATH="$HOME/bin:$PATH"
来源：http://grw.hnxiangtu.top

[R76] 使用临时文件
来源：http://gcj.ydzc1.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hoc.sxryk.cn

[R77] 读取用户输入
来源：http://vin.0kj1m.cn

read -rp "请输入: " ans
来源：http://muw.yueranfly.top

[R78] 交互式菜单
来源：http://wif.dianchejie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yrg.wangshuangyany.cn

[R79] 解析命令行选项
来源：http://ygw.316326.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jki.epnwcf.com

[R80] 查看脚本执行耗时
来源：http://prd.birdmap.top

time ./run.sh
来源：http://zgy.0kj1m.cn

================================================================================
来源：http://bop.havefunace.top

S. C / C++ 专题
来源：http://ywe.ywan-chungtsiang.top

================================================================================
来源：http://wbx.bbcook.cn

[S01] C：Hello World
来源：http://hkp.guowangkeji.top

#include <stdio.h>
来源：http://jgu.zhaomingkeji.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://swy.c1oappe.top

[S02] C：变量与格式化输出
来源：http://chv.hammf.cn

int a = 10; printf("%d\n", a);
来源：http://tlr.aibaodan.cn

[S03] C：读入整数
来源：http://qrk.jinqigfzy.top

int x; scanf("%d", &x);
来源：http://wsi.cheryme.top

[S04] C：字符串复制
来源：http://mwm.snrcjt.cn

char dst[32]; strcpy(dst, "hi");
来源：http://grx.yj20258.top

[S05] C：字符串长度
来源：http://btg.yj20258.top

strlen(s)
来源：http://ymp.hammf.cn

[S06] C：字符串比较
来源：http://ukl.epnwcf.com

strcmp(a, b) == 0
来源：http://mwv.birdmap.top

[S07] C：数组遍历求和
来源：http://ozb.ydjk.org.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yrf.daria6918.cn

[S08] C：动态内存分配与释放
来源：http://ltn.meibo888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wls.yj20258888.top

[S09] C：结构体定义与初始化
来源：http://joj.ppjwa.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yzj.ivvv.top

[S10] C：指针与解引用
来源：http://ewt.c1oappe.top

int *p = &a;  *p = 5;
来源：http://njn.yj202588.top

[S11] C：逐行读文件
来源：http://uic.tanke756.top

FILE *f = fopen("a.txt", "r");
来源：http://zys.c1oappe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qok.cashguo.top

fclose(f);
来源：http://bgi.yonumen.top

[S12] C：写文件
来源：http://ryu.xuetiantiany.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fti.havefunace.top

[S13] C：宏定义
来源：http://sjc.jinqigufen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dux.jinghuilouyu.cn

[S14] C：枚举
来源：http://yex.zhengqikj.top

enum Color { RED, GREEN, BLUE };
来源：http://uuo.sufxvd.cn

[S15] C：类型转换
来源：http://wtv.hongshengwenyu.top

(double) a / b
来源：http://tqq.xuanzx.com

[S16] C：位操作置位
来源：http://pqp.wangdashe.top

x |= (1 << 3);
来源：http://pfa.0kj1m.cn

[S17] C：安全拼接字符串
来源：http://ulk.zdbjq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fup.shangyingyoupin.top

[S18] C：命令行参数
来源：http://btv.chenlongwang.top

int main(int argc, char **argv)
来源：http://wam.shanyushiyangtech.top

[S19] C：快速排序
来源：http://orq.hywenlv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zxo.0kj1m.cn

[S20] C：二分查找
来源：http://ljy.gzhubu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pwn.yvedp.cn

[S21] C：字符类别判断
来源：http://dkh.tanke756.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dxq.yfazqb.com

[S22] C：字符串转数字
来源：http://aaj.hywenlv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://grb.yonumen.top

[S23] C：随机数
来源：http://dkn.xylfe.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ips.sjlbkw.cn

[S24] C：获取本地时间
来源：http://men.dianchejie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://evl.ppjwa.cn

[S25] C：内存拷贝
来源：http://ajs.hcnkem.com

memcpy(dst, src, n);
来源：http://xxa.svipenyu.cn

[S26] C：内存清零
来源：http://ybv.uphjek.com

memset(a, 0, sizeof a);
来源：http://xjy.svipenyu.cn

[S27] C：定义常量
来源：http://iag.ctjpmb.com

const double PI = 3.14159;
来源：http://yqh.tarul.cn

[S28] C：静态变量
来源：http://xnu.feifeiyinyue.top


<!-- 参考信息 -->