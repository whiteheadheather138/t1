代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://fqc.hammf.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qgh.jqgfzy.top

[Q43] 标量子查询
来源：http://qbb.redwolf501.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lzt.gogol.net.cn

[Q44] IN 子查询
来源：http://dkp.jianghu66.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://euz.cashguo.top

[Q45] EXISTS 判断存在
来源：http://eat.quarkkingdee.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fag.aizwys.cn

[Q46] NOT EXISTS 判断不存在
来源：http://twf.mhx1999.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tgo.zhixingplan.top

[Q47] 与平均值比较
来源：http://esd.cdnleiting.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qex.wangdashe.top

[Q48] CTE 公用表表达式
来源：http://geq.zhiwuduotai.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uzy.gogol.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://rxj.hesvh.cn

[Q49] 更新单行
来源：http://tft.ivvv.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dpx.havefunace.top

[Q50] 批量更新
来源：http://ldm.pycfn.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lqq.0kj1m.cn

[Q51] 用子查询更新
来源：http://izc.aibaodan.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wqw.chenlongwang.top

[Q52] 删除指定行
来源：http://cfv.gzhubu.top

DELETE FROM users WHERE id = 10;
来源：http://ubc.andypj.xyz

[Q53] 按条件删除
来源：http://qzy.fktsv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fpa.hongshengwenyu.top

[Q54] 清空表
来源：http://wxk.cheryme.top

TRUNCATE TABLE logs;
来源：http://qlw.yanxiufei.cn

[Q55] 排名（并列占位）
来源：http://kbb.sysykeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ymn.c1oappe.top

[Q56] 密集排名（并列不占位）
来源：http://fzr.vehdjk.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ekl.guowangkeji.top

[Q57] 行号
来源：http://ilx.hnqzz.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vyx.guannengcc.top

[Q58] 累计求和
来源：http://cpw.zhiwuduotai.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hdj.xinyue.icu

[Q59] 分组内累计
来源：http://gxb.xinyue.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jfi.epnwcf.com

[Q60] 取上一行 / 下一行
来源：http://yck.fanxiaobao.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qrz.shuidangran.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mxf.meibo888.top

[Q61] 移动平均
来源：http://ydy.aibaodan.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uce.hnxiangtu.top

[Q62] 分组占比
来源：http://ohg.ehwqpu.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kfn.zdqjudy.top

[Q63] 开启事务
来源：http://okl.nanxuanxn.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tjg.iojbl.cn

[Q64] 提交事务
来源：http://poh.mhx1999.top

COMMIT;
来源：http://wfm.hnqzz.top

[Q65] 回滚事务
来源：http://abw.jinqigfzy.top

ROLLBACK;
来源：http://kkr.hongshengwenyu.top

[Q66] 行锁查询
来源：http://rqq.yueranfly.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oif.zhongyouzk.top

[Q67] 设置隔离级别
来源：http://maj.jiagoushi.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nte.zycfv.cn

[Q68] 保存点
来源：http://lct.fzhhl.top

SAVEPOINT sp1;
来源：http://ibh.sweek.top

ROLLBACK TO sp1;
来源：http://lcl.jyoumei.cn

[Q69] 查看执行计划
来源：http://vcm.fehbvm.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sjv.epnwcf.com

[Q70] 更新统计信息
来源：http://vsq.zdbjq.cn

ANALYZE TABLE users;
来源：http://upm.c1oappe.top

[Q71] 查看建表语句
来源：http://jqm.chenjidiqi.icu

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://urf.vehdjk.com

[Q72] 查看索引
来源：http://puk.9152youxi.cn

SHOW INDEX FROM users;
来源：http://bkp.pycfn.com

[Q73] 查看表状态
来源：http://hii.hesvh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hsg.zycfv.cn

[Q74] 强制使用索引
来源：http://wtv.yangfankeji.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://byn.dashuyun.cn

[Q75] 日期格式化
来源：http://mcn.yj20258888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ymd.vehdjk.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kdc.xziqi.cn

[Q76] 按天统计
来源：http://jex.ybcxt.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hco.fanxiaobao.xyz

[Q77] 时间加减
来源：http://sdo.sufxvd.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mee.fanxiaobao.xyz

[Q78] 当前时间
来源：http://mhn.fzhhl.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mlb.tian-w.cn

[Q79] 字符串拼接
来源：http://cxn.meibo888.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://roj.zhoulong.xyz

[Q80] 字符串截取
来源：http://pxy.gaohongyu789.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://szy.cucudq.cn

[Q81] 字符串替换
来源：http://rjl.chenjidiqi.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bbu.tian-w.cn

[Q82] 字符长度与字节长度
来源：http://glp.hnxiangtu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://scv.redwolf501.top

[Q83] 大小写转换
来源：http://lfg.gaohongyu789.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jjp.0kj1m.cn

[Q84] 去除首尾空格
来源：http://fju.sxryk.cn

SELECT TRIM(name) FROM users;
来源：http://ltx.havefunace.top

[Q85] 数值取整
来源：http://ghi.yvedp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tsl.ydzc1.top

[Q86] 读取 JSON 字段
来源：http://hqo.ehwqpu.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fky.xinyue.icu

[Q87] JSON 字段做条件
来源：http://vlw.yj20258.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qug.52xcode.cn

[Q88] 行转列（条件聚合）
来源：http://loi.mhx1999.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ocb.chenzaomai.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ibb.sjlbkw.cn

[Q89] 判断表是否存在
来源：http://hjo.gzhubu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pbx.nanxinkj.top

[Q90] 生成序号列
来源：http://mpa.bbcook.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jfg.vqdsnc.cn

================================================================================
来源：http://rmr.jinqigufen.top

R. Bash 专题
来源：http://pqd.hnqzz.top

================================================================================
来源：http://fno.ywan-chungtsiang.top

[R01] shebang 与严格模式
来源：http://kpj.dashuyun.cn

#!/usr/bin/env bash
来源：http://kbc.ehwqpu.com

set -euo pipefail
来源：http://uyg.hnxiangtu.top

[R02] 变量赋值与使用
来源：http://ljf.52xcode.cn

name="Tom"; echo "$name"
来源：http://mmi.vqdsnc.cn

[R03] 只读变量
来源：http://oni.gzhubu.top

readonly PI=3.14
来源：http://dpz.zhiwuduotai.top

[R04] 位置参数
来源：http://xgq.yuxming.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://aax.ywan-chungtsiang.top

[R05] 参数默认值
来源：http://arf.nwbrower.top

name="${1:-default}"
来源：http://xry.jinyuanbaomall.cn

[R06] 判断命令是否存在
来源：http://ddc.hnqzz.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qfs.hnqzz.top

[R07] if 判断文件
来源：http://ins.xylfe.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pah.fehbvm.com

[R08] 数值比较
来源：http://omx.wangshuangyany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jrj.tian-w.cn

[R09] 字符串比较
来源：http://hqo.yj202588.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wzy.cashguo.top

[R10] 正则匹配
来源：http://kbn.nanxinkj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mvc.mhx1999.top

[R11] case 多分支
来源：http://ukb.guannengcc.top

case "$1" in
来源：http://fpl.sxryk.cn

start) echo "启动" ;;
来源：http://eko.hysaishi.cn

stop)  echo "停止" ;;
来源：http://oeq.xingfuxueyuan.xyz

*)     echo "未知命令" ;;
来源：http://vgj.kuanghao11.cn

esac
来源：http://wmp.jinghuilouyu.cn

[R12] for 遍历文件
来源：http://pjo.jinghuilouyu.cn

for f in *.txt; do echo "$f"; done
来源：http://jki.cashguo.top

[R13] for 计数循环
来源：http://uqp.ehwqpu.com

for i in {1..10}; do echo "$i"; done
来源：http://knr.xinyue.icu

[R14] C 风格 for
来源：http://oat.jianghu66.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aex.sufxvd.cn

[R15] while 逐行读文件
来源：http://aek.wangshuangyany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://szy.vqdsnc.cn

[R16] until 等待条件
来源：http://hwl.ywan-chungtsiang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://guy.yvedp.cn

[R17] 数组定义与取值
来源：http://zlh.hnqzz.top

arr=(a b c); echo "${arr[0]}"
来源：http://vgw.shanyushiyangtech.top

[R18] 遍历数组
来源：http://mfv.yj202588.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uah.sxryk.cn

[R19] 数组长度
来源：http://dhs.birdmap.top

echo "${#arr[@]}"
来源：http://kst.zhixingplan.top

[R20] 关联数组（字典）
来源：http://dnk.sysykeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oea.chenlongwang.top

[R21] 字符串长度
来源：http://zlk.ehwqpu.com

echo "${#s}"
来源：http://vnx.gotoacloud.top

[R22] 截取子串
来源：http://rwh.guannengcc.top

echo "${s:0:5}"
来源：http://xjm.jinyuanbaomall.cn

[R23] 字符串替换
来源：http://zla.fehbvm.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hdd.ppjwa.cn

[R24] 大小写转换
来源：http://ubd.bbcook.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ukx.snrcjt.cn

[R25] 去后缀 / 去前缀
来源：http://rvj.zhoulong.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://omj.jinqigufen.top

[R26] 命令替换
来源：http://qix.dianchejie.cn

now=$(date +%F); echo "$now"
来源：http://gui.pengpengdd.cyou

[R27] 算术展开
来源：http://mvq.havefunace.top

echo $((1 + 2 * 3))
来源：http://jrh.iojbl.cn

[R28] 浮点运算
来源：http://hid.gaohongyu789.top

echo "scale=2; 10/3" | bc
来源：http://jou.jqgfzy.top

[R29] 定义函数
来源：http://gyx.tanke756.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://diq.cqqwz.cn

[R30] 函数返回状态码
来源：http://dtg.fzhhl.top

f() { return 0; }; f || echo "失败了"
来源：http://ubk.tian-w.cn

[R31] 局部变量
来源：http://lxz.shanyushiyangkeji.top

f() { local x=1; echo "$x"; }
来源：http://ieb.cheryme.top

[R32] 参数个数校验
来源：http://hsc.zhijiandao.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cig.wangshuangyany.cn

[R33] 捕获错误并提示行号
来源：http://mci.shuidangran.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tzf.jinqigfzy.top

[R34] 退出时清理
来源：http://oge.ydzc1.top

trap 'rm -f "$tmp"' EXIT
来源：http://jrk.jinyuanbaomall.cn

[R35] 后台执行并等待
来源：http://qjj.sufxvd.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kiy.jyoumei.cn

[R36] 并发执行多个任务
来源：http://jfd.ctjpmb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ztu.hnxiangtu.top

[R37] 把输出赋给变量
来源：http://ntj.9152youxi.cn

files=$(ls -1)
来源：http://rcr.cdnleiting.top

[R38] 管道串联
来源：http://ycg.aibaodan.cn

cat a.txt | grep -i error | wc -l
来源：http://mdx.jinqigufen.top

[R39] 重定向标准输出与错误
来源：http://dqg.yanxiufei.cn

cmd > out.log 2>&1
来源：http://byf.jinqigufen.top

[R40] 追加写日志
来源：http://efr.smart0.xyz

echo "log" >> out.log
来源：http://ypd.chenlongwang.top

[R41] 丢弃输出
来源：http://hbj.ivvv.top

cmd >/dev/null 2>&1
来源：http://pcc.jqgfzy.top

[R42] 输入重定向
来源：http://lyd.shuidangran.top

wc -l < a.txt
来源：http://ntj.zdbjq.cn

[R43] 按名字查找文件
来源：http://psp.sysykeji.top

find . -name "*.log" -type f
来源：http://aoe.sweek.top

[R44] 按修改时间查找
来源：http://aoc.sufxvd.cn

find . -mtime -7 -type f
来源：http://rhh.fanxiaobao.xyz

[R45] 批量删除
来源：http://hqv.sufxvd.cn

find . -name "*.tmp" -delete
来源：http://usb.jinghuilouyu.cn

[R46] 递归替换文件内容
来源：http://cux.tanke756.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dma.cqqwz.cn

[R47] sed 单行替换
来源：http://est.fanxiaobao.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://qgw.epnwcf.com

[R48] awk 取指定列
来源：http://lcw.xuetiantiany.cn

awk '{print $1, $3}' a.txt
来源：http://cpi.wangshuangyany.cn

[R49] awk 带条件
来源：http://ncu.zdbjq.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ncv.daxiang520.top

[R50] awk 求和
来源：http://sqk.yangfankeji.com

awk '{s += $2} END {print s}' a.txt
来源：http://xqe.daxiang520.top

[R51] 排序去重取前几
来源：http://wcw.vqdsnc.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hqm.nanxuanxn.top

[R52] 统计行数
来源：http://exl.cdnleiting.top

wc -l a.txt
来源：http://ick.havefunace.top

[R53] 查看文件头与实时尾
来源：http://xef.shzxlz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xab.cheryme.top

[R54] 比较两个文件
来源：http://jvw.yangfankeji.com

diff a.txt b.txt
来源：http://orp.ctjpmb.com

[R55] 压缩与解压
来源：http://kko.shanyushiyangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://raz.0kj1m.cn

[R56] 远程拷贝
来源：http://ygi.ydjk.org.cn

scp file user@host:/path/
来源：http://wyv.uphjek.com

[R57] 远程执行命令
来源：http://wph.mhx1999.top

ssh user@host 'uptime'
来源：http://nvg.dashuyun.cn

[R58] 下载文件
来源：http://ipw.jinqigfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bsz.wangdashe.top

[R59] 发 POST JSON
来源：http://qyi.redwolf501.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jdc.hysaishi.cn

[R60] 只看 HTTP 状态码
来源：http://tso.fehbvm.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kkd.shanyushiyangkeji.top

[R61] 磁盘占用
来源：http://yui.shuidangran.top

df -h;  du -sh *
来源：http://nas.bjfxy.top

[R62] 找最占空间的文件
来源：http://pec.yueranfly.top

du -ah . | sort -rh | head -10
来源：http://uno.yj20258888.top

[R63] 内存与进程
来源：http://ydb.vqdsnc.cn

free -h;  ps aux | grep nginx
来源：http://fst.zhoulong.xyz

[R64] 结束进程
来源：http://vty.chenzaomai.com

kill -9 $(pgrep -f app.py)
来源：http://rnd.sweek.top

[R65] 查看端口占用
来源：http://nqg.xziqi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://npv.ybcxt.top

[R66] 定时任务
来源：http://jrh.shanyushiyangkeji.top

crontab -e;  crontab -l
来源：http://crp.52xcode.cn

[R67] 生成随机十六进制串
来源：http://ohy.ydjk.org.cn

openssl rand -hex 16
来源：http://jsn.quarkkingdee.top

[R68] 计算文件校验值
来源：http://cic.yvedp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://eyn.chenzaomai.com

[R69] 生成随机密码
来源：http://icc.zhongyouzk.top

head -c 16 /dev/urandom | base64
来源：http://pol.yanxiufei.cn

[R70] 时间戳与互转
来源：http://dwb.yj202588.top

date +%s;  date -d @1700000000
来源：http://kej.chenzaomai.com

[R71] 日期格式化
来源：http://fid.yj20258888.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bns.zdqjudy.top

[R72] 等待端口就绪
来源：http://rzh.gotoacloud.top

until nc -z localhost 3306; do sleep 1; done
来源：http://eaa.daria6918.cn

[R73] 分割大日志
来源：http://nfx.chenzaomai.com

split -l 1000 big.log part_
来源：http://unf.yonumen.top

[R74] 批量重命名
来源：http://odm.yuanzhike.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vxn.vehdjk.com

[R75] 导出环境变量
来源：http://ixb.guowangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://tlx.52xcode.cn

[R76] 使用临时文件
来源：http://ezf.redwolf501.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wja.jinghuilouyu.cn

[R77] 读取用户输入
来源：http://ahz.jinqigfzy.top

read -rp "请输入: " ans
来源：http://jwr.yangfankeji.com

[R78] 交互式菜单
来源：http://xzk.0kj1m.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zpt.jqgufenzy.top

[R79] 解析命令行选项
来源：http://cxu.cqqwz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://euh.xuetiantiany.cn

[R80] 查看脚本执行耗时
来源：http://fsc.uphjek.com

time ./run.sh
来源：http://zbi.jinqigufen.top

================================================================================
来源：http://ruq.vqdsnc.cn

S. C / C++ 专题
来源：http://mmz.gogol.net.cn

================================================================================
来源：http://caj.xziqi.cn

[S01] C：Hello World
来源：http://klm.cucudq.cn

#include <stdio.h>
来源：http://klk.cdnleiting.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://who.yj202588.top

[S02] C：变量与格式化输出
来源：http://par.c1oappe.top

int a = 10; printf("%d\n", a);
来源：http://zjd.haohaochexian.top

[S03] C：读入整数
来源：http://qnr.yvedp.cn

int x; scanf("%d", &x);
来源：http://kgn.0kj1m.cn

[S04] C：字符串复制
来源：http://bse.mhx1999.top

char dst[32]; strcpy(dst, "hi");
来源：http://adv.fanxiaobao.xyz

[S05] C：字符串长度
来源：http://qtw.chenzaomai.com

strlen(s)
来源：http://grb.guannengcc.top

[S06] C：字符串比较
来源：http://pog.9152youxi.cn

strcmp(a, b) == 0
来源：http://nmd.gaohongyu789.top

[S07] C：数组遍历求和
来源：http://xec.feifeiyinyue.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vod.fzhhl.top

[S08] C：动态内存分配与释放
来源：http://aqk.shuidangran.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qxf.snrcjt.cn

[S09] C：结构体定义与初始化
来源：http://lsr.zhijiandao.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://avi.daxiang520.top

[S10] C：指针与解引用
来源：http://zpk.xingfuxueyuan.xyz

int *p = &a;  *p = 5;
来源：http://omr.chenzaomai.com

[S11] C：逐行读文件
来源：http://fyr.fanxiaobao.xyz

FILE *f = fopen("a.txt", "r");
来源：http://iqv.yongpay.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://eap.yongpay.top

fclose(f);
来源：http://gmm.ivvv.top

[S12] C：写文件
来源：http://lgn.wangdashe.top


<!-- 参考信息 -->