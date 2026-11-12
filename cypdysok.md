代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://prl.cdnleiting.top

[Q32] 分组拼接字符串
来源：http://elx.guowangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qot.iojbl.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ikb.birdmap.top

[Q33] 多列分组
来源：http://xtj.zhoulong.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ets.hesvh.cn

[Q34] 每组取第一条
来源：http://aqt.snrcjt.cn

SELECT * FROM (
来源：http://aoj.nanxinkj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fye.cucudq.cn

) t WHERE rn = 1;
来源：http://dkf.fengsongda.top

[Q35] 内连接
来源：http://cdq.daria6918.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hma.jinyuanbaomall.cn

[Q36] 左连接
来源：http://drq.chenjidiqi.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wnn.ydzc1.top

[Q37] 右连接
来源：http://unr.andypj.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xju.smart0.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://wrg.hnxiangtu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bwn.dianchejie.cn

[Q39] 自连接（查上下级）
来源：http://ozw.nanxinkj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ayw.ywan-chungtsiang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://eia.cdnleiting.top

[Q40] 交叉连接（笛卡尔积）
来源：http://orr.redwolf501.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mhr.9152youxi.cn

[Q41] 多表连接
来源：http://acb.shzxlz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yji.hnqzz.top

JOIN users u ON u.id = o.user_id
来源：http://quj.sweek.top

JOIN products p ON p.id = o.product_id;
来源：http://tok.gzhubu.top

[Q42] 连接条件附加过滤
来源：http://jpt.yangfankeji.com

SELECT u.name, o.amount FROM users u
来源：http://wlb.xuanzx.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mab.zhoulong.xyz

[Q43] 标量子查询
来源：http://spo.gotoacloud.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baw.quarkkingdee.top

[Q44] IN 子查询
来源：http://suc.c1oappe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dve.gogol.net.cn

[Q45] EXISTS 判断存在
来源：http://utu.fzhhl.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hbw.jinqigfzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://itx.xingfuxueyuan.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ndu.hfpthk.cn

[Q47] 与平均值比较
来源：http://tea.feifeiyinyue.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cgq.ivvv.top

[Q48] CTE 公用表表达式
来源：http://ive.mhx1999.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tzm.zhijiandao.cn

SELECT * FROM t WHERE c > 5;
来源：http://pcv.hywenlv.cn

[Q49] 更新单行
来源：http://fib.iojbl.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uam.yueranfly.top

[Q50] 批量更新
来源：http://klx.yanxiufei.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fgu.nwbrower.top

[Q51] 用子查询更新
来源：http://rji.dashuyun.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sps.xinyue.icu

[Q52] 删除指定行
来源：http://xly.chenjidiqi.icu

DELETE FROM users WHERE id = 10;
来源：http://lud.redwolf501.top

[Q53] 按条件删除
来源：http://cmt.smart0.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vyi.wangshuangyany.cn

[Q54] 清空表
来源：http://tde.jqgufenzy.top

TRUNCATE TABLE logs;
来源：http://swr.andypj.xyz

[Q55] 排名（并列占位）
来源：http://jep.wangshuangyany.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zmc.hnqzz.top

[Q56] 密集排名（并列不占位）
来源：http://vhv.sweek.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uyw.zhengqikj.top

[Q57] 行号
来源：http://nax.yfazqb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ent.birdmap.top

[Q58] 累计求和
来源：http://tbr.aizwys.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cue.zhongyouzk.top

[Q59] 分组内累计
来源：http://mcb.0kj1m.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vez.shuidangran.top

[Q60] 取上一行 / 下一行
来源：http://voo.wangshuangyany.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://znq.chenjidiqi.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jux.yj202588.top

[Q61] 移动平均
来源：http://tri.aibaodan.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wms.guannengcc.top

[Q62] 分组占比
来源：http://vkb.hysaishi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kxl.snrcjt.cn

[Q63] 开启事务
来源：http://nry.ydzc1.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ndr.feifeiyinyue.top

[Q64] 提交事务
来源：http://qyl.ehwqpu.com

COMMIT;
来源：http://nch.xingfuxueyuan.xyz

[Q65] 回滚事务
来源：http://vva.smart0.xyz

ROLLBACK;
来源：http://ohj.guannengcc.top

[Q66] 行锁查询
来源：http://bhf.ppjwa.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ftc.redwolf501.top

[Q67] 设置隔离级别
来源：http://bxw.shzxlz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kuz.svipenyu.cn

[Q68] 保存点
来源：http://dom.jinghuilouyu.cn

SAVEPOINT sp1;
来源：http://biy.xingfuxueyuan.xyz

ROLLBACK TO sp1;
来源：http://rqh.tian-w.cn

[Q69] 查看执行计划
来源：http://bkg.hcnkem.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dbw.yj20258888.top

[Q70] 更新统计信息
来源：http://uqz.ctjpmb.com

ANALYZE TABLE users;
来源：http://lpi.snrcjt.cn

[Q71] 查看建表语句
来源：http://loi.ehwqpu.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://djv.kuanghao11.cn

[Q72] 查看索引
来源：http://mnj.gaohongyu789.top

SHOW INDEX FROM users;
来源：http://drp.xziqi.cn

[Q73] 查看表状态
来源：http://kry.sweek.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vml.hcnkem.com

[Q74] 强制使用索引
来源：http://ndj.yuxming.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sst.epnwcf.com

[Q75] 日期格式化
来源：http://lxt.zdqjudy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wjn.sweek.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://biu.hnqzz.top

[Q76] 按天统计
来源：http://ckj.chenzaomai.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ngl.jinqigfzy.top

[Q77] 时间加减
来源：http://oul.jlsjyb.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nlz.guowangkeji.top

[Q78] 当前时间
来源：http://vup.hongshengwenyu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://boy.yangfankeji.com

[Q79] 字符串拼接
来源：http://kyl.dashuyun.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ypa.shanyushiyangtech.top

[Q80] 字符串截取
来源：http://vzh.tarul.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://obb.52xcode.cn

[Q81] 字符串替换
来源：http://ndc.tian-w.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qaf.gzhubu.top

[Q82] 字符长度与字节长度
来源：http://wnd.jqgufenzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hto.chenzaomai.com

[Q83] 大小写转换
来源：http://zcr.uphjek.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nqy.nanxuanxn.top

[Q84] 去除首尾空格
来源：http://rif.yangfankeji.com

SELECT TRIM(name) FROM users;
来源：http://ywe.nwbrower.top

[Q85] 数值取整
来源：http://rse.hesvh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://muu.birdmap.top

[Q86] 读取 JSON 字段
来源：http://ezl.ydzc1.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bne.fehbvm.com

[Q87] JSON 字段做条件
来源：http://qio.wangdashe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qze.zdbjq.cn

[Q88] 行转列（条件聚合）
来源：http://ylh.xingfuxueyuan.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xxk.bjfxy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://adu.zhixingplan.top

[Q89] 判断表是否存在
来源：http://jhw.hammf.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jsz.tian-w.cn

[Q90] 生成序号列
来源：http://fut.svipenyu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qly.gotoacloud.top

================================================================================
来源：http://cut.yueranfly.top

R. Bash 专题
来源：http://pik.fktsv.cn

================================================================================
来源：http://bhk.uphjek.com

[R01] shebang 与严格模式
来源：http://nuj.jqgufenzy.top

#!/usr/bin/env bash
来源：http://kzf.yuanzhike.top

set -euo pipefail
来源：http://ydi.jinqigfzy.top

[R02] 变量赋值与使用
来源：http://fbs.c1oappe.top

name="Tom"; echo "$name"
来源：http://ixj.jqgufenzy.top

[R03] 只读变量
来源：http://qro.yfazqb.com

readonly PI=3.14
来源：http://gcp.jianghu66.top

[R04] 位置参数
来源：http://gdy.yanxiufei.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://obb.zdqjudy.top

[R05] 参数默认值
来源：http://wkf.dianchejie.cn

name="${1:-default}"
来源：http://pth.sysykeji.top

[R06] 判断命令是否存在
来源：http://jcm.aizwys.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ngh.sysykeji.top

[R07] if 判断文件
来源：http://aww.uphjek.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jvr.aizwys.cn

[R08] 数值比较
来源：http://dny.xinyue.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://znx.shuidangran.top

[R09] 字符串比较
来源：http://fqd.cdnleiting.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mxr.fengsongda.top

[R10] 正则匹配
来源：http://pki.tianlin.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qsw.fanxiaobao.xyz

[R11] case 多分支
来源：http://yrr.fktsv.cn

case "$1" in
来源：http://uhr.nanxinkj.top

start) echo "启动" ;;
来源：http://yyi.zhengqikj.top

stop)  echo "停止" ;;
来源：http://yvr.daxiang520.top

*)     echo "未知命令" ;;
来源：http://tpb.jlsjyb.cn

esac
来源：http://vlq.jiagoushi.top

[R12] for 遍历文件
来源：http://lqd.dianchejie.cn

for f in *.txt; do echo "$f"; done
来源：http://npy.c1oappe.top

[R13] for 计数循环
来源：http://pdk.jinqigfzy.top

for i in {1..10}; do echo "$i"; done
来源：http://yrs.cashguo.top

[R14] C 风格 for
来源：http://gms.dashuyun.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wwo.vehdjk.com

[R15] while 逐行读文件
来源：http://mwp.mhx1999.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tnh.pengpengdd.cyou

[R16] until 等待条件
来源：http://dkj.zdbjq.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vdy.shangyingyoupin.top

[R17] 数组定义与取值
来源：http://hoj.ybcxt.top

arr=(a b c); echo "${arr[0]}"
来源：http://uqj.zycfv.cn

[R18] 遍历数组
来源：http://qms.yonumen.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xqb.zhengqikj.top

[R19] 数组长度
来源：http://emo.ywan-chungtsiang.top

echo "${#arr[@]}"
来源：http://vwz.gaohongyu789.top

[R20] 关联数组（字典）
来源：http://xpx.jinghuilouyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lwe.jqgufenzy.top

[R21] 字符串长度
来源：http://tyi.gaohongyu789.top

echo "${#s}"
来源：http://xqs.haohaochexian.top

[R22] 截取子串
来源：http://ujg.guowangkeji.top

echo "${s:0:5}"
来源：http://lff.jqgufenzy.top

[R23] 字符串替换
来源：http://lhg.zhengqikj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pyh.hcnkem.com

[R24] 大小写转换
来源：http://avv.tarul.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qug.xziqi.cn

[R25] 去后缀 / 去前缀
来源：http://eli.yfazqb.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://oad.shuidangran.top

[R26] 命令替换
来源：http://zqa.birdmap.top

now=$(date +%F); echo "$now"
来源：http://pqz.yueranfly.top

[R27] 算术展开
来源：http://qqj.jiagoushi.top

echo $((1 + 2 * 3))
来源：http://kus.quarkkingdee.top

[R28] 浮点运算
来源：http://obi.meibo888.top

echo "scale=2; 10/3" | bc
来源：http://urt.yongpay.top

[R29] 定义函数
来源：http://nob.cqqwz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wyh.shzxlz.cn

[R30] 函数返回状态码
来源：http://yoy.zhijiandao.cn

f() { return 0; }; f || echo "失败了"
来源：http://sur.iojbl.cn

[R31] 局部变量
来源：http://rtt.guowangkeji.top

f() { local x=1; echo "$x"; }
来源：http://bmz.jinyuanbaomall.cn

[R32] 参数个数校验
来源：http://scu.yuanzhike.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://utl.cashguo.top

[R33] 捕获错误并提示行号
来源：http://tnq.iojbl.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nzu.jinghuilouyu.cn

[R34] 退出时清理
来源：http://urt.aizwys.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ctx.xingfuxueyuan.xyz

[R35] 后台执行并等待
来源：http://utg.jinghuilouyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oyx.jqgufenzy.top

[R36] 并发执行多个任务
来源：http://hhq.gotoacloud.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blg.yangfankeji.com

[R37] 把输出赋给变量
来源：http://lpz.shanyushiyangkeji.top

files=$(ls -1)
来源：http://zgi.fengsongda.top

[R38] 管道串联
来源：http://aez.ywan-chungtsiang.top

cat a.txt | grep -i error | wc -l
来源：http://fbq.yongpay.top

[R39] 重定向标准输出与错误
来源：http://qfq.zdbjq.cn

cmd > out.log 2>&1
来源：http://xtw.feifeiyinyue.top

[R40] 追加写日志
来源：http://zxv.gaohongyu789.top

echo "log" >> out.log
来源：http://rnk.daria6918.cn

[R41] 丢弃输出
来源：http://htv.yonumen.top

cmd >/dev/null 2>&1
来源：http://xrs.jlsjyb.cn

[R42] 输入重定向
来源：http://qui.dashuyun.cn

wc -l < a.txt
来源：http://fhw.ivvv.top

[R43] 按名字查找文件
来源：http://xhu.aizwys.cn

find . -name "*.log" -type f
来源：http://osz.havefunace.top

[R44] 按修改时间查找
来源：http://qnu.jqgufenzy.top

find . -mtime -7 -type f
来源：http://rhv.chenlongwang.top

[R45] 批量删除
来源：http://pda.birdmap.top

find . -name "*.tmp" -delete
来源：http://rta.hnqzz.top

[R46] 递归替换文件内容
来源：http://cpi.jianghu66.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mmb.tanke756.top

[R47] sed 单行替换
来源：http://qfb.kuanghao11.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bkn.0kj1m.cn

[R48] awk 取指定列
来源：http://fhd.zhengqikj.top

awk '{print $1, $3}' a.txt
来源：http://wyz.fanxiaobao.xyz

[R49] awk 带条件
来源：http://iyp.yfazqb.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qmt.pengpengdd.cyou

[R50] awk 求和
来源：http://qbb.jinyuanbaomall.cn

awk '{s += $2} END {print s}' a.txt
来源：http://plf.jiagoushi.top

[R51] 排序去重取前几
来源：http://oao.sjlbkw.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tdv.iojbl.cn

[R52] 统计行数
来源：http://wkd.fengsongda.top

wc -l a.txt
来源：http://zxt.xinyue.icu

[R53] 查看文件头与实时尾
来源：http://bes.ywan-chungtsiang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://eev.guowangkeji.top

[R54] 比较两个文件
来源：http://tsf.aibaodan.cn

diff a.txt b.txt
来源：http://nyv.guowangkeji.top

[R55] 压缩与解压
来源：http://juc.yj20258.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yvt.hfpthk.cn

[R56] 远程拷贝
来源：http://scp.pengpengdd.cyou

scp file user@host:/path/
来源：http://cnv.hnxiangtu.top

[R57] 远程执行命令
来源：http://oph.xuetiantiany.cn

ssh user@host 'uptime'
来源：http://usn.cucudq.cn

[R58] 下载文件
来源：http://zxc.smart0.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lzk.yangfankeji.com

[R59] 发 POST JSON
来源：http://ron.zhoulong.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://guc.gogol.net.cn

[R60] 只看 HTTP 状态码
来源：http://rzn.daxiang520.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fah.0kj1m.cn

[R61] 磁盘占用
来源：http://zmp.hcnkem.com

df -h;  du -sh *
来源：http://iic.zhoulong.xyz

[R62] 找最占空间的文件
来源：http://fyi.0kj1m.cn

du -ah . | sort -rh | head -10
来源：http://fgt.yj20258888.top

[R63] 内存与进程
来源：http://fsb.chenzaomai.com

free -h;  ps aux | grep nginx
来源：http://fbc.andypj.xyz

[R64] 结束进程
来源：http://mhs.zhijiandao.cn

kill -9 $(pgrep -f app.py)
来源：http://cxw.c1oappe.top

[R65] 查看端口占用
来源：http://zwj.0kj1m.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ojq.c1oappe.top

[R66] 定时任务
来源：http://zum.nanxinkj.top

crontab -e;  crontab -l
来源：http://wom.yueranfly.top

[R67] 生成随机十六进制串
来源：http://vfb.pengpengdd.cyou

openssl rand -hex 16
来源：http://igw.gzhubu.top

[R68] 计算文件校验值
来源：http://nyh.fanxiaobao.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://hii.aizwys.cn

[R69] 生成随机密码
来源：http://lir.pengpengdd.cyou

head -c 16 /dev/urandom | base64
来源：http://wha.pycfn.com

[R70] 时间戳与互转
来源：http://bzz.nanxinkj.top

date +%s;  date -d @1700000000
来源：http://jfm.wangdashe.top

[R71] 日期格式化
来源：http://dra.yanxiufei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yqy.zhoulong.xyz

[R72] 等待端口就绪
来源：http://oev.cqqwz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uon.zdqjudy.top

[R73] 分割大日志
来源：http://bba.cheryme.top

split -l 1000 big.log part_
来源：http://zxb.zdbjq.cn

[R74] 批量重命名
来源：http://bgi.hammf.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iqd.chenzaomai.com

[R75] 导出环境变量
来源：http://qal.yonumen.top

export PATH="$HOME/bin:$PATH"
来源：http://fhs.fktsv.cn

[R76] 使用临时文件
来源：http://fdt.ctjpmb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mgu.fengsongda.top

[R77] 读取用户输入
来源：http://rcf.sysykeji.top

read -rp "请输入: " ans
来源：http://koo.wangshuangyany.cn

[R78] 交互式菜单
来源：http://dph.xziqi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xjz.chenjidiqi.icu

[R79] 解析命令行选项
来源：http://lyc.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kax.sxryk.cn

[R80] 查看脚本执行耗时
来源：http://qvr.xuetiantiany.cn

time ./run.sh
来源：http://irp.fehbvm.com

================================================================================
来源：http://phi.yongpay.top


<!-- 参考信息 -->