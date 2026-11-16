代发 wailian999

[Q36] 左连接
来源：http://mhf.smart0.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eez.fanxiaobao.xyz

[Q37] 右连接
来源：http://meb.uphjek.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hti.hesvh.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jmv.chenlongwang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cdo.tianlin.xyz

[Q39] 自连接（查上下级）
来源：http://cqc.ivvv.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://icd.jinghuilouyu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mpb.nanxuanxn.top

[Q40] 交叉连接（笛卡尔积）
来源：http://skw.yuanzhike.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://krl.pengpengdd.cyou

[Q41] 多表连接
来源：http://bna.yj20258.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://dpt.yj20258888.top

JOIN users u ON u.id = o.user_id
来源：http://vuc.chenjidiqi.icu

JOIN products p ON p.id = o.product_id;
来源：http://giu.epnwcf.com

[Q42] 连接条件附加过滤
来源：http://dct.hysaishi.cn

SELECT u.name, o.amount FROM users u
来源：http://dbr.gogol.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zeg.quarkkingdee.top

[Q43] 标量子查询
来源：http://jpj.fengsongda.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lvc.yuanzhike.top

[Q44] IN 子查询
来源：http://edp.hnqzz.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yor.9152youxi.cn

[Q45] EXISTS 判断存在
来源：http://wtf.jqgfzy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xgh.sweek.top

[Q46] NOT EXISTS 判断不存在
来源：http://fce.cdnleiting.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://drk.yj20258888.top

[Q47] 与平均值比较
来源：http://rqk.bbcook.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eul.meibo888.top

[Q48] CTE 公用表表达式
来源：http://pza.9152youxi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ouk.yangfankeji.com

SELECT * FROM t WHERE c > 5;
来源：http://rmc.jinyuanbaomall.cn

[Q49] 更新单行
来源：http://tew.jyoumei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sxe.aibaodan.cn

[Q50] 批量更新
来源：http://zog.zhengqikj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://czw.hongshengwenyu.top

[Q51] 用子查询更新
来源：http://kmf.cucudq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nnc.pycfn.com

[Q52] 删除指定行
来源：http://jrz.yfazqb.com

DELETE FROM users WHERE id = 10;
来源：http://qnx.epnwcf.com

[Q53] 按条件删除
来源：http://utn.zhiwuduotai.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ekf.bjfxy.top

[Q54] 清空表
来源：http://rix.hnqzz.top

TRUNCATE TABLE logs;
来源：http://mku.tarul.cn

[Q55] 排名（并列占位）
来源：http://zwl.zhixingplan.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wzy.andypj.xyz

[Q56] 密集排名（并列不占位）
来源：http://bbv.xziqi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uff.jinqigfzy.top

[Q57] 行号
来源：http://eus.daria6918.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rpb.ydjk.org.cn

[Q58] 累计求和
来源：http://rcy.cucudq.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://urp.ctjpmb.com

[Q59] 分组内累计
来源：http://gkg.birdmap.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ilg.cqqwz.cn

[Q60] 取上一行 / 下一行
来源：http://rer.yuanzhike.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://okx.shanyushiyangtech.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pmr.yj202588.top

[Q61] 移动平均
来源：http://cne.ivvv.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uty.xylfe.cn

[Q62] 分组占比
来源：http://iph.ybcxt.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oum.gaohongyu789.top

[Q63] 开启事务
来源：http://xon.svipenyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nne.yanxiufei.cn

[Q64] 提交事务
来源：http://biu.yangfankeji.com

COMMIT;
来源：http://aqx.jiagoushi.top

[Q65] 回滚事务
来源：http://svd.ydzc1.top

ROLLBACK;
来源：http://zga.ybcxt.top

[Q66] 行锁查询
来源：http://shd.hammf.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qep.vehdjk.com

[Q67] 设置隔离级别
来源：http://jpe.hesvh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yog.ctjpmb.com

[Q68] 保存点
来源：http://mwi.jqgfzy.top

SAVEPOINT sp1;
来源：http://bgn.zhaomingkeji.xyz

ROLLBACK TO sp1;
来源：http://mgv.fengsongda.top

[Q69] 查看执行计划
来源：http://kqq.bjfxy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gir.jianghu66.top

[Q70] 更新统计信息
来源：http://seq.cucudq.cn

ANALYZE TABLE users;
来源：http://eoq.shanyushiyangkeji.top

[Q71] 查看建表语句
来源：http://wpl.zhoulong.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ivx.ybcxt.top

[Q72] 查看索引
来源：http://rha.dashuyun.cn

SHOW INDEX FROM users;
来源：http://thv.shzxlz.cn

[Q73] 查看表状态
来源：http://aog.hysaishi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ohu.xziqi.cn

[Q74] 强制使用索引
来源：http://jhg.zhaomingkeji.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qha.andypj.xyz

[Q75] 日期格式化
来源：http://nwy.jinghuilouyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hul.yuxming.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://erf.zhongyouzk.top

[Q76] 按天统计
来源：http://lhy.yuanzhike.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://non.jqgfzy.top

[Q77] 时间加减
来源：http://zma.wangshuangyany.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uun.jqgfzy.top

[Q78] 当前时间
来源：http://gxm.mhx1999.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://frh.zhijiandao.cn

[Q79] 字符串拼接
来源：http://inn.nanxuanxn.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fhb.chenjidiqi.icu

[Q80] 字符串截取
来源：http://bes.xylfe.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nba.hcnkem.com

[Q81] 字符串替换
来源：http://msf.fktsv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://shf.yj20258888.top

[Q82] 字符长度与字节长度
来源：http://azm.aibaodan.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eto.daria6918.cn

[Q83] 大小写转换
来源：http://uok.gaohongyu789.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yvb.ivvv.top

[Q84] 去除首尾空格
来源：http://zmt.316326.xyz

SELECT TRIM(name) FROM users;
来源：http://sqz.chenlongwang.top

[Q85] 数值取整
来源：http://inh.xuetiantiany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ipy.cucudq.cn

[Q86] 读取 JSON 字段
来源：http://klt.sjlbkw.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://znn.kuanghao11.cn

[Q87] JSON 字段做条件
来源：http://oeq.uphjek.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mkv.shanyushiyangtech.top

[Q88] 行转列（条件聚合）
来源：http://wwf.hysaishi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dgb.0kj1m.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dhl.sweek.top

[Q89] 判断表是否存在
来源：http://cbx.gotoacloud.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://emj.shzxlz.cn

[Q90] 生成序号列
来源：http://fps.aibaodan.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hnq.zhengqikj.top

================================================================================
来源：http://gwc.svipenyu.cn

R. Bash 专题
来源：http://kao.bbcook.cn

================================================================================
来源：http://ykw.ivvv.top

[R01] shebang 与严格模式
来源：http://vqh.tarul.cn

#!/usr/bin/env bash
来源：http://ukk.smart0.xyz

set -euo pipefail
来源：http://fth.cashguo.top

[R02] 变量赋值与使用
来源：http://ilr.haohaochexian.top

name="Tom"; echo "$name"
来源：http://cxl.jinqigfzy.top

[R03] 只读变量
来源：http://rja.pengpengdd.cyou

readonly PI=3.14
来源：http://cum.ehwqpu.com

[R04] 位置参数
来源：http://fur.daxiang520.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kjc.hcnkem.com

[R05] 参数默认值
来源：http://nff.jinqigufen.top

name="${1:-default}"
来源：http://hcv.sufxvd.cn

[R06] 判断命令是否存在
来源：http://xit.jinqigfzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nbm.zhengqikj.top

[R07] if 判断文件
来源：http://rpr.sweek.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fbg.ivvv.top

[R08] 数值比较
来源：http://lmq.zhongyouzk.top

if (( a > b )); then echo "a 更大"; fi
来源：http://frs.gzhubu.top

[R09] 字符串比较
来源：http://rsk.aizwys.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ecc.ybcxt.top

[R10] 正则匹配
来源：http://kdp.xuanzx.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mhs.andypj.xyz

[R11] case 多分支
来源：http://vyl.cheryme.top

case "$1" in
来源：http://mxf.yuxming.cn

start) echo "启动" ;;
来源：http://ago.yongpay.top

stop)  echo "停止" ;;
来源：http://nln.iojbl.cn

*)     echo "未知命令" ;;
来源：http://fcg.xinyue.icu

esac
来源：http://jxe.chenlongwang.top

[R12] for 遍历文件
来源：http://rev.xuetiantiany.cn

for f in *.txt; do echo "$f"; done
来源：http://ztn.xylfe.cn

[R13] for 计数循环
来源：http://ebv.hnqzz.top

for i in {1..10}; do echo "$i"; done
来源：http://etv.nanxinkj.top

[R14] C 风格 for
来源：http://hxa.zhoulong.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bdf.tianlin.xyz

[R15] while 逐行读文件
来源：http://lyv.xylfe.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pcz.316326.xyz

[R16] until 等待条件
来源：http://pak.gaohongyu789.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nam.tanke756.top

[R17] 数组定义与取值
来源：http://iyd.aizwys.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bep.aizwys.cn

[R18] 遍历数组
来源：http://xsd.hcnkem.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wjt.ydjk.org.cn

[R19] 数组长度
来源：http://qjz.316326.xyz

echo "${#arr[@]}"
来源：http://vwe.meibo888.top

[R20] 关联数组（字典）
来源：http://blx.guowangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://iwb.jiagoushi.top

[R21] 字符串长度
来源：http://crw.hysaishi.cn

echo "${#s}"
来源：http://vzr.pycfn.com

[R22] 截取子串
来源：http://wqb.yvedp.cn

echo "${s:0:5}"
来源：http://fvo.jinghuilouyu.cn

[R23] 字符串替换
来源：http://lpr.jinghuilouyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wbw.aizwys.cn

[R24] 大小写转换
来源：http://ycs.yfazqb.com

echo "${s^^}"; echo "${s,,}"
来源：http://ugt.yangfankeji.com

[R25] 去后缀 / 去前缀
来源：http://pbt.wangshuangyany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://avk.aizwys.cn

[R26] 命令替换
来源：http://uyh.hammf.cn

now=$(date +%F); echo "$now"
来源：http://nkz.iojbl.cn

[R27] 算术展开
来源：http://idc.shuidangran.top

echo $((1 + 2 * 3))
来源：http://wqz.zhongyouzk.top

[R28] 浮点运算
来源：http://asf.zdbjq.cn

echo "scale=2; 10/3" | bc
来源：http://tru.andypj.xyz

[R29] 定义函数
来源：http://ewr.zycfv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://edo.ehwqpu.com

[R30] 函数返回状态码
来源：http://iad.xziqi.cn

f() { return 0; }; f || echo "失败了"
来源：http://uei.redwolf501.top

[R31] 局部变量
来源：http://czx.xuetiantiany.cn

f() { local x=1; echo "$x"; }
来源：http://sdw.smart0.xyz

[R32] 参数个数校验
来源：http://srq.ydzc1.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jjy.yuxming.cn

[R33] 捕获错误并提示行号
来源：http://fzp.hnqzz.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vkx.zhijiandao.cn

[R34] 退出时清理
来源：http://czw.svipenyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://krd.hongshengwenyu.top

[R35] 后台执行并等待
来源：http://lse.chenjidiqi.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://lhb.jinghuilouyu.cn

[R36] 并发执行多个任务
来源：http://fin.gotoacloud.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kri.aizwys.cn

[R37] 把输出赋给变量
来源：http://exq.mhx1999.top

files=$(ls -1)
来源：http://ozd.tian-w.cn

[R38] 管道串联
来源：http://ldm.ppjwa.cn

cat a.txt | grep -i error | wc -l
来源：http://aqg.zdqjudy.top

[R39] 重定向标准输出与错误
来源：http://wvx.pycfn.com

cmd > out.log 2>&1
来源：http://koi.ywan-chungtsiang.top

[R40] 追加写日志
来源：http://yps.fktsv.cn

echo "log" >> out.log
来源：http://yhk.dianchejie.cn

[R41] 丢弃输出
来源：http://dks.jinqigfzy.top

cmd >/dev/null 2>&1
来源：http://bhd.zdqjudy.top

[R42] 输入重定向
来源：http://tvn.chenlongwang.top

wc -l < a.txt
来源：http://aku.sufxvd.cn

[R43] 按名字查找文件
来源：http://pel.sysykeji.top

find . -name "*.log" -type f
来源：http://ryh.cqqwz.cn

[R44] 按修改时间查找
来源：http://gds.chenjidiqi.icu

find . -mtime -7 -type f
来源：http://mlt.ehwqpu.com

[R45] 批量删除
来源：http://osr.zhiwuduotai.top

find . -name "*.tmp" -delete
来源：http://vao.yj20258.top

[R46] 递归替换文件内容
来源：http://eav.cqqwz.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ips.tianlin.xyz

[R47] sed 单行替换
来源：http://aha.hnxiangtu.top

sed -i 's/foo/bar/g' a.txt
来源：http://yad.yongpay.top

[R48] awk 取指定列
来源：http://sry.bbcook.cn

awk '{print $1, $3}' a.txt
来源：http://udj.0kj1m.cn

[R49] awk 带条件
来源：http://hsa.shuidangran.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iyk.dianchejie.cn

[R50] awk 求和
来源：http://vpw.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://nqw.jiagoushi.top

[R51] 排序去重取前几
来源：http://ubq.yueranfly.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hza.ydjk.org.cn

[R52] 统计行数
来源：http://kxw.ivvv.top

wc -l a.txt
来源：http://hcd.zhengqikj.top

[R53] 查看文件头与实时尾
来源：http://jha.ywan-chungtsiang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vys.jinghuilouyu.cn

[R54] 比较两个文件
来源：http://zdc.hnxiangtu.top

diff a.txt b.txt
来源：http://lam.ywan-chungtsiang.top

[R55] 压缩与解压
来源：http://ddh.9152youxi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://drv.wangdashe.top

[R56] 远程拷贝
来源：http://prc.kuanghao11.cn

scp file user@host:/path/
来源：http://tmd.quarkkingdee.top

[R57] 远程执行命令
来源：http://ngk.cheryme.top

ssh user@host 'uptime'
来源：http://zww.chenzaomai.com

[R58] 下载文件
来源：http://dzo.yanxiufei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pzd.jinqigufen.top

[R59] 发 POST JSON
来源：http://ibe.gzhubu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qmb.fktsv.cn

[R60] 只看 HTTP 状态码
来源：http://nba.yueranfly.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://skt.xuanzx.com

[R61] 磁盘占用
来源：http://mbs.zhaomingkeji.xyz

df -h;  du -sh *
来源：http://zid.birdmap.top

[R62] 找最占空间的文件
来源：http://wpk.ydzc1.top

du -ah . | sort -rh | head -10
来源：http://giw.vehdjk.com

[R63] 内存与进程
来源：http://mtv.yvedp.cn

free -h;  ps aux | grep nginx
来源：http://tcj.yuanzhike.top

[R64] 结束进程
来源：http://sok.snrcjt.cn

kill -9 $(pgrep -f app.py)
来源：http://gax.nanxuanxn.top

[R65] 查看端口占用
来源：http://tan.yj20258.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ksa.yueranfly.top

[R66] 定时任务
来源：http://auc.wangshuangyany.cn

crontab -e;  crontab -l
来源：http://aeo.zhaomingkeji.xyz

[R67] 生成随机十六进制串
来源：http://yfb.xingfuxueyuan.xyz

openssl rand -hex 16
来源：http://rsw.sweek.top

[R68] 计算文件校验值
来源：http://ask.chenjidiqi.icu

sha256sum a.txt;  md5sum a.txt
来源：http://pau.jlsjyb.cn

[R69] 生成随机密码
来源：http://oqx.jinyuanbaomall.cn

head -c 16 /dev/urandom | base64
来源：http://dlv.ywan-chungtsiang.top

[R70] 时间戳与互转
来源：http://rbp.cucudq.cn

date +%s;  date -d @1700000000
来源：http://fjj.shangyingyoupin.top

[R71] 日期格式化
来源：http://bra.mhx1999.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mik.andypj.xyz

[R72] 等待端口就绪
来源：http://pls.jianghu66.top

until nc -z localhost 3306; do sleep 1; done
来源：http://csp.smart0.xyz

[R73] 分割大日志
来源：http://xty.jinqigufen.top

split -l 1000 big.log part_
来源：http://uzx.jinyuanbaomall.cn

[R74] 批量重命名
来源：http://wsp.hysaishi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gyg.jinghuilouyu.cn

[R75] 导出环境变量
来源：http://gao.birdmap.top

export PATH="$HOME/bin:$PATH"
来源：http://feu.0kj1m.cn

[R76] 使用临时文件
来源：http://qvv.sxryk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wne.jinqigfzy.top

[R77] 读取用户输入
来源：http://rkl.hnqzz.top

read -rp "请输入: " ans
来源：http://nzc.yfazqb.com

[R78] 交互式菜单
来源：http://wvs.svipenyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pub.ydjk.org.cn

[R79] 解析命令行选项
来源：http://gqn.dianchejie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://psk.xuanzx.com

[R80] 查看脚本执行耗时
来源：http://ckq.shangyingyoupin.top

time ./run.sh
来源：http://wsj.epnwcf.com

================================================================================
来源：http://ohn.nanxuanxn.top

S. C / C++ 专题
来源：http://yga.hongshengwenyu.top

================================================================================
来源：http://etm.shuidangran.top

[S01] C：Hello World
来源：http://crq.birdmap.top

#include <stdio.h>
来源：http://stk.zycfv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://clu.yvedp.cn

[S02] C：变量与格式化输出
来源：http://pmg.zhongyouzk.top

int a = 10; printf("%d\n", a);
来源：http://gqp.fanxiaobao.xyz

[S03] C：读入整数
来源：http://loy.meibo888.top

int x; scanf("%d", &x);
来源：http://ipf.ywan-chungtsiang.top

[S04] C：字符串复制
来源：http://wem.ppjwa.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wkj.yj20258888.top

[S05] C：字符串长度
来源：http://ngi.guowangkeji.top


<!-- 参考信息 -->