代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wjs.tarul.cn

[Q52] 删除指定行
来源：http://aax.52xcode.cn

DELETE FROM users WHERE id = 10;
来源：http://aku.mhx1999.top

[Q53] 按条件删除
来源：http://kly.chenzaomai.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vpk.pengpengdd.cyou

[Q54] 清空表
来源：http://ggw.xylfe.cn

TRUNCATE TABLE logs;
来源：http://apd.smart0.xyz

[Q55] 排名（并列占位）
来源：http://sjx.chenlongwang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hfe.sxryk.cn

[Q56] 密集排名（并列不占位）
来源：http://bgr.mhx1999.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uoc.chenzaomai.com

[Q57] 行号
来源：http://uur.pengpengdd.cyou

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kyu.ivvv.top

[Q58] 累计求和
来源：http://uly.hywenlv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nle.nanxinkj.top

[Q59] 分组内累计
来源：http://yuz.epnwcf.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fhf.tarul.cn

[Q60] 取上一行 / 下一行
来源：http://wjz.yfazqb.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vto.havefunace.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tyn.ywan-chungtsiang.top

[Q61] 移动平均
来源：http://nuk.zdqjudy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ijz.ydzc1.top

[Q62] 分组占比
来源：http://ejk.cqqwz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jvu.fanxiaobao.xyz

[Q63] 开启事务
来源：http://ais.yj202588.top

START TRANSACTION;                -- 或 BEGIN
来源：http://nrc.uphjek.com

[Q64] 提交事务
来源：http://wbo.zhiwuduotai.top

COMMIT;
来源：http://mfs.hcnkem.com

[Q65] 回滚事务
来源：http://hxj.snrcjt.cn

ROLLBACK;
来源：http://bza.hywenlv.cn

[Q66] 行锁查询
来源：http://boi.dianchejie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zjo.jinqigufen.top

[Q67] 设置隔离级别
来源：http://xkf.xuetiantiany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://szi.yuanzhike.top

[Q68] 保存点
来源：http://kwv.zhoulong.xyz

SAVEPOINT sp1;
来源：http://mcl.chenzaomai.com

ROLLBACK TO sp1;
来源：http://mur.cucudq.cn

[Q69] 查看执行计划
来源：http://ebe.chenzaomai.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zqh.cashguo.top

[Q70] 更新统计信息
来源：http://nbi.haohaochexian.top

ANALYZE TABLE users;
来源：http://vbo.zhoulong.xyz

[Q71] 查看建表语句
来源：http://qqt.nwbrower.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://npe.hysaishi.cn

[Q72] 查看索引
来源：http://bye.fktsv.cn

SHOW INDEX FROM users;
来源：http://vsx.cucudq.cn

[Q73] 查看表状态
来源：http://jpz.jqgufenzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jcm.shuidangran.top

[Q74] 强制使用索引
来源：http://ere.ydjk.org.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ukg.snrcjt.cn

[Q75] 日期格式化
来源：http://riq.mhx1999.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://acf.yongpay.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gju.9152youxi.cn

[Q76] 按天统计
来源：http://uvx.jinqigufen.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hum.zhoulong.xyz

[Q77] 时间加减
来源：http://nne.ywan-chungtsiang.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://okv.zhijiandao.cn

[Q78] 当前时间
来源：http://nvc.cdnleiting.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nnp.uphjek.com

[Q79] 字符串拼接
来源：http://xgn.ydzc1.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kzz.guannengcc.top

[Q80] 字符串截取
来源：http://riu.ydzc1.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://euw.sxryk.cn

[Q81] 字符串替换
来源：http://luj.yueranfly.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hdb.gogol.net.cn

[Q82] 字符长度与字节长度
来源：http://ufu.zhiwuduotai.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jml.0kj1m.cn

[Q83] 大小写转换
来源：http://xrv.hesvh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cew.fehbvm.com

[Q84] 去除首尾空格
来源：http://twk.gogol.net.cn

SELECT TRIM(name) FROM users;
来源：http://bgt.cdnleiting.top

[Q85] 数值取整
来源：http://ygo.shzxlz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ulg.guannengcc.top

[Q86] 读取 JSON 字段
来源：http://qxa.tarul.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qey.hesvh.cn

[Q87] JSON 字段做条件
来源：http://xyh.xuetiantiany.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kfn.jianghu66.top

[Q88] 行转列（条件聚合）
来源：http://kpd.hnqzz.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://agx.meibo888.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kxd.yuanzhike.top

[Q89] 判断表是否存在
来源：http://buv.vehdjk.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://loc.cheryme.top

[Q90] 生成序号列
来源：http://lbz.sysykeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wbm.haohaochexian.top

================================================================================
来源：http://pbv.feifeiyinyue.top

R. Bash 专题
来源：http://vhs.yueranfly.top

================================================================================
来源：http://lng.quarkkingdee.top

[R01] shebang 与严格模式
来源：http://qcw.cucudq.cn

#!/usr/bin/env bash
来源：http://abn.yj20258888.top

set -euo pipefail
来源：http://hjw.yfazqb.com

[R02] 变量赋值与使用
来源：http://uwd.hysaishi.cn

name="Tom"; echo "$name"
来源：http://slx.cashguo.top

[R03] 只读变量
来源：http://zyc.daxiang520.top

readonly PI=3.14
来源：http://ezf.chenzaomai.com

[R04] 位置参数
来源：http://bsu.guowangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://srf.bbcook.cn

[R05] 参数默认值
来源：http://lpv.uphjek.com

name="${1:-default}"
来源：http://crq.gaohongyu789.top

[R06] 判断命令是否存在
来源：http://gkw.gogol.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xxg.jqgufenzy.top

[R07] if 判断文件
来源：http://imj.gaohongyu789.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://svu.dashuyun.cn

[R08] 数值比较
来源：http://rmo.hongshengwenyu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://lag.pycfn.com

[R09] 字符串比较
来源：http://nkz.chenlongwang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ghy.jinghuilouyu.cn

[R10] 正则匹配
来源：http://sdk.jiagoushi.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://syw.zhengqikj.top

[R11] case 多分支
来源：http://lrn.jinqigufen.top

case "$1" in
来源：http://ilk.tanke756.top

start) echo "启动" ;;
来源：http://lpx.jqgfzy.top

stop)  echo "停止" ;;
来源：http://ibt.gaohongyu789.top

*)     echo "未知命令" ;;
来源：http://hcw.tianlin.xyz

esac
来源：http://mqt.aibaodan.cn

[R12] for 遍历文件
来源：http://eit.pengpengdd.cyou

for f in *.txt; do echo "$f"; done
来源：http://aer.yvedp.cn

[R13] for 计数循环
来源：http://pym.yongpay.top

for i in {1..10}; do echo "$i"; done
来源：http://uly.fanxiaobao.xyz

[R14] C 风格 for
来源：http://eqe.aizwys.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pno.hysaishi.cn

[R15] while 逐行读文件
来源：http://tfo.0kj1m.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xwm.birdmap.top

[R16] until 等待条件
来源：http://cmr.zhoulong.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://khw.chenlongwang.top

[R17] 数组定义与取值
来源：http://dtu.yvedp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rgx.fzhhl.top

[R18] 遍历数组
来源：http://fcv.shanyushiyangtech.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jsm.daria6918.cn

[R19] 数组长度
来源：http://ugj.yonumen.top

echo "${#arr[@]}"
来源：http://wqz.zycfv.cn

[R20] 关联数组（字典）
来源：http://vrl.snrcjt.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://war.havefunace.top

[R21] 字符串长度
来源：http://qhs.zycfv.cn

echo "${#s}"
来源：http://jmm.hnqzz.top

[R22] 截取子串
来源：http://wng.sufxvd.cn

echo "${s:0:5}"
来源：http://suw.hnqzz.top

[R23] 字符串替换
来源：http://awf.zhijiandao.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ndl.sxryk.cn

[R24] 大小写转换
来源：http://oym.xinyue.icu

echo "${s^^}"; echo "${s,,}"
来源：http://jjc.guowangkeji.top

[R25] 去后缀 / 去前缀
来源：http://psz.epnwcf.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://zsa.fengsongda.top

[R26] 命令替换
来源：http://tql.zycfv.cn

now=$(date +%F); echo "$now"
来源：http://ldm.9152youxi.cn

[R27] 算术展开
来源：http://pgf.birdmap.top

echo $((1 + 2 * 3))
来源：http://zqb.hnxiangtu.top

[R28] 浮点运算
来源：http://jyz.mhx1999.top

echo "scale=2; 10/3" | bc
来源：http://bei.zdqjudy.top

[R29] 定义函数
来源：http://jyd.hywenlv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vqt.nwbrower.top

[R30] 函数返回状态码
来源：http://jag.guowangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://gpc.shangyingyoupin.top

[R31] 局部变量
来源：http://exh.yuxming.cn

f() { local x=1; echo "$x"; }
来源：http://wop.xinyue.icu

[R32] 参数个数校验
来源：http://mwu.feifeiyinyue.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hnb.zhijiandao.cn

[R33] 捕获错误并提示行号
来源：http://qut.zhijiandao.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://saf.dashuyun.cn

[R34] 退出时清理
来源：http://hqt.c1oappe.top

trap 'rm -f "$tmp"' EXIT
来源：http://uky.daxiang520.top

[R35] 后台执行并等待
来源：http://ppw.haohaochexian.top

sleep 5 & pid=$!; wait "$pid"
来源：http://els.9152youxi.cn

[R36] 并发执行多个任务
来源：http://izv.iojbl.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://abt.xingfuxueyuan.xyz

[R37] 把输出赋给变量
来源：http://bzk.jqgufenzy.top

files=$(ls -1)
来源：http://phs.quarkkingdee.top

[R38] 管道串联
来源：http://lto.ywan-chungtsiang.top

cat a.txt | grep -i error | wc -l
来源：http://yku.jqgfzy.top

[R39] 重定向标准输出与错误
来源：http://mnz.fzhhl.top

cmd > out.log 2>&1
来源：http://cka.hnqzz.top

[R40] 追加写日志
来源：http://boo.yj202588.top

echo "log" >> out.log
来源：http://msm.yj20258.top

[R41] 丢弃输出
来源：http://haw.smart0.xyz

cmd >/dev/null 2>&1
来源：http://mld.daria6918.cn

[R42] 输入重定向
来源：http://irs.hfpthk.cn

wc -l < a.txt
来源：http://fzy.cucudq.cn

[R43] 按名字查找文件
来源：http://cka.daria6918.cn

find . -name "*.log" -type f
来源：http://yvp.9152youxi.cn

[R44] 按修改时间查找
来源：http://jdl.jinqigfzy.top

find . -mtime -7 -type f
来源：http://cyk.316326.xyz

[R45] 批量删除
来源：http://kmj.yfazqb.com

find . -name "*.tmp" -delete
来源：http://oer.fehbvm.com

[R46] 递归替换文件内容
来源：http://hyn.shuidangran.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bda.redwolf501.top

[R47] sed 单行替换
来源：http://cel.shanyushiyangtech.top

sed -i 's/foo/bar/g' a.txt
来源：http://dkc.yvedp.cn

[R48] awk 取指定列
来源：http://frd.wangshuangyany.cn

awk '{print $1, $3}' a.txt
来源：http://iuu.svipenyu.cn

[R49] awk 带条件
来源：http://ufj.gotoacloud.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://itc.c1oappe.top

[R50] awk 求和
来源：http://tmh.hysaishi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bec.jinqigfzy.top

[R51] 排序去重取前几
来源：http://okt.sufxvd.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rul.jinghuilouyu.cn

[R52] 统计行数
来源：http://flr.jinghuilouyu.cn

wc -l a.txt
来源：http://czj.pengpengdd.cyou

[R53] 查看文件头与实时尾
来源：http://cmj.yonumen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sxu.yueranfly.top

[R54] 比较两个文件
来源：http://nwt.uphjek.com

diff a.txt b.txt
来源：http://vxx.yj20258888.top

[R55] 压缩与解压
来源：http://ftt.tarul.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xpn.ppjwa.cn

[R56] 远程拷贝
来源：http://ajq.haohaochexian.top

scp file user@host:/path/
来源：http://flf.xingfuxueyuan.xyz

[R57] 远程执行命令
来源：http://dqt.yj20258888.top

ssh user@host 'uptime'
来源：http://szi.gogol.net.cn

[R58] 下载文件
来源：http://ssr.nanxuanxn.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://liy.jqgufenzy.top

[R59] 发 POST JSON
来源：http://qsi.iojbl.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gyj.9152youxi.cn

[R60] 只看 HTTP 状态码
来源：http://osw.hnxiangtu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iqn.yj20258.top

[R61] 磁盘占用
来源：http://zkd.jqgfzy.top

df -h;  du -sh *
来源：http://sfn.aizwys.cn

[R62] 找最占空间的文件
来源：http://qpf.haohaochexian.top

du -ah . | sort -rh | head -10
来源：http://arb.shanyushiyangtech.top

[R63] 内存与进程
来源：http://cxo.sjlbkw.cn

free -h;  ps aux | grep nginx
来源：http://yfh.hywenlv.cn

[R64] 结束进程
来源：http://mow.wangshuangyany.cn

kill -9 $(pgrep -f app.py)
来源：http://hko.hfpthk.cn

[R65] 查看端口占用
来源：http://kso.sufxvd.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://piu.zycfv.cn

[R66] 定时任务
来源：http://vjt.guannengcc.top

crontab -e;  crontab -l
来源：http://kfw.tanke756.top

[R67] 生成随机十六进制串
来源：http://mmt.yuanzhike.top

openssl rand -hex 16
来源：http://kpc.0kj1m.cn

[R68] 计算文件校验值
来源：http://peh.ppjwa.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bav.c1oappe.top

[R69] 生成随机密码
来源：http://mzu.chenjidiqi.icu

head -c 16 /dev/urandom | base64
来源：http://mrr.sjlbkw.cn

[R70] 时间戳与互转
来源：http://kpq.smart0.xyz

date +%s;  date -d @1700000000
来源：http://nsv.jinqigfzy.top

[R71] 日期格式化
来源：http://pda.ydjk.org.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zyt.xinyue.icu

[R72] 等待端口就绪
来源：http://ygr.xylfe.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://naq.wangdashe.top

[R73] 分割大日志
来源：http://qau.zhoulong.xyz

split -l 1000 big.log part_
来源：http://kxs.jinqigfzy.top

[R74] 批量重命名
来源：http://yjb.sjlbkw.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cic.bbcook.cn

[R75] 导出环境变量
来源：http://epc.uphjek.com

export PATH="$HOME/bin:$PATH"
来源：http://fqn.xinyue.icu

[R76] 使用临时文件
来源：http://bip.wangshuangyany.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hfx.gotoacloud.top

[R77] 读取用户输入
来源：http://cgg.ywan-chungtsiang.top

read -rp "请输入: " ans
来源：http://occ.xinyue.icu

[R78] 交互式菜单
来源：http://hix.cdnleiting.top

select opt in a b c; do echo "$opt"; break; done
来源：http://pwo.sufxvd.cn

[R79] 解析命令行选项
来源：http://mjy.jinyuanbaomall.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cls.hnqzz.top

[R80] 查看脚本执行耗时
来源：http://igi.kuanghao11.cn

time ./run.sh
来源：http://ees.kuanghao11.cn

================================================================================
来源：http://vzh.haohaochexian.top

S. C / C++ 专题
来源：http://jbe.hnxiangtu.top

================================================================================
来源：http://fhw.guowangkeji.top

[S01] C：Hello World
来源：http://paz.xingfuxueyuan.xyz

#include <stdio.h>
来源：http://eju.hnxiangtu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://yrf.aibaodan.cn

[S02] C：变量与格式化输出
来源：http://cci.fehbvm.com

int a = 10; printf("%d\n", a);
来源：http://nyh.zhongyouzk.top

[S03] C：读入整数
来源：http://qns.yfazqb.com

int x; scanf("%d", &x);
来源：http://lrm.ybcxt.top

[S04] C：字符串复制
来源：http://fcm.gotoacloud.top

char dst[32]; strcpy(dst, "hi");
来源：http://bfa.iojbl.cn

[S05] C：字符串长度
来源：http://acn.yueranfly.top

strlen(s)
来源：http://ael.birdmap.top

[S06] C：字符串比较
来源：http://daf.chenlongwang.top

strcmp(a, b) == 0
来源：http://tth.wangdashe.top

[S07] C：数组遍历求和
来源：http://dbn.gotoacloud.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tlx.ybcxt.top

[S08] C：动态内存分配与释放
来源：http://yhj.tanke756.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pns.nanxuanxn.top

[S09] C：结构体定义与初始化
来源：http://avb.nanxuanxn.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ltl.fzhhl.top

[S10] C：指针与解引用
来源：http://xke.yangfankeji.com

int *p = &a;  *p = 5;
来源：http://jpr.jiagoushi.top

[S11] C：逐行读文件
来源：http://olw.daxiang520.top

FILE *f = fopen("a.txt", "r");
来源：http://dtz.cqqwz.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ehg.jinghuilouyu.cn

fclose(f);
来源：http://xlt.hongshengwenyu.top

[S12] C：写文件
来源：http://xlw.haohaochexian.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cav.tarul.cn

[S13] C：宏定义
来源：http://kul.gzhubu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dtu.fengsongda.top

[S14] C：枚举
来源：http://ubp.shanyushiyangtech.top

enum Color { RED, GREEN, BLUE };
来源：http://muh.chenlongwang.top

[S15] C：类型转换
来源：http://fin.wangshuangyany.cn

(double) a / b
来源：http://yyd.hnqzz.top

[S16] C：位操作置位
来源：http://ito.sxryk.cn

x |= (1 << 3);
来源：http://jqh.pengpengdd.cyou

[S17] C：安全拼接字符串
来源：http://xwm.chenjidiqi.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tou.hongshengwenyu.top

[S18] C：命令行参数
来源：http://oha.hywenlv.cn

int main(int argc, char **argv)
来源：http://tbw.52xcode.cn

[S19] C：快速排序
来源：http://ejh.cdnleiting.top

qsort(a, n, sizeof(int), cmp);
来源：http://dvt.xingfuxueyuan.xyz

[S20] C：二分查找
来源：http://txe.gotoacloud.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sox.xziqi.cn

[S21] C：字符类别判断
来源：http://wjf.xuanzx.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://djq.yongpay.top

[S22] C：字符串转数字
来源：http://tho.gotoacloud.top


<!-- 参考信息 -->