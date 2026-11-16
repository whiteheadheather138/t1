代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pqf.sufxvd.cn

[Q26] 计数
来源：http://dux.jqgufenzy.top

SELECT COUNT(*) FROM users;
来源：http://hjo.gotoacloud.top

[Q27] 条件计数
来源：http://rjc.shzxlz.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://twm.chenlongwang.top

[Q28] 求和与平均
来源：http://jgy.havefunace.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wuw.aizwys.cn

[Q29] 最大最小值
来源：http://dbb.bbcook.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ehy.gaohongyu789.top

[Q30] 分组统计
来源：http://rdi.jinqigfzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wjl.yuanzhike.top

[Q31] 分组后过滤
来源：http://dxy.yangfankeji.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://syy.hesvh.cn

[Q32] 分组拼接字符串
来源：http://xgg.aizwys.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://erm.gaohongyu789.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ewn.zdbjq.cn

[Q33] 多列分组
来源：http://xyb.dianchejie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://csd.ydzc1.top

[Q34] 每组取第一条
来源：http://rdk.0kj1m.cn

SELECT * FROM (
来源：http://kqq.jinghuilouyu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wtj.hcnkem.com

) t WHERE rn = 1;
来源：http://ssd.0kj1m.cn

[Q35] 内连接
来源：http://skx.tanke756.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://apz.tanke756.top

[Q36] 左连接
来源：http://krv.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uun.aizwys.cn

[Q37] 右连接
来源：http://shx.gogol.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ujh.uphjek.com

[Q38] 全外连接（PostgreSQL）
来源：http://edv.hnxiangtu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bex.xingfuxueyuan.xyz

[Q39] 自连接（查上下级）
来源：http://lrt.bbcook.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kvw.zdqjudy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mwn.yonumen.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hac.ppjwa.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wzw.kuanghao11.cn

[Q41] 多表连接
来源：http://eof.uphjek.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://emm.jinghuilouyu.cn

JOIN users u ON u.id = o.user_id
来源：http://pfy.0kj1m.cn

JOIN products p ON p.id = o.product_id;
来源：http://smk.daxiang520.top

[Q42] 连接条件附加过滤
来源：http://gnu.yfazqb.com

SELECT u.name, o.amount FROM users u
来源：http://zmx.jianghu66.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xle.dashuyun.cn

[Q43] 标量子查询
来源：http://kbn.ehwqpu.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qro.zhoulong.xyz

[Q44] IN 子查询
来源：http://tws.smart0.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blm.iojbl.cn

[Q45] EXISTS 判断存在
来源：http://uvs.c1oappe.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ykg.ppjwa.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xwc.shzxlz.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cpc.hesvh.cn

[Q47] 与平均值比较
来源：http://faa.zhongyouzk.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dws.hysaishi.cn

[Q48] CTE 公用表表达式
来源：http://lfp.gzhubu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ulv.sxryk.cn

SELECT * FROM t WHERE c > 5;
来源：http://gwi.zhongyouzk.top

[Q49] 更新单行
来源：http://ywn.ppjwa.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hhi.pycfn.com

[Q50] 批量更新
来源：http://mzn.daria6918.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lvv.ywan-chungtsiang.top

[Q51] 用子查询更新
来源：http://hhw.nwbrower.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mqy.wangshuangyany.cn

[Q52] 删除指定行
来源：http://dto.chenjidiqi.icu

DELETE FROM users WHERE id = 10;
来源：http://uqy.jinyuanbaomall.cn

[Q53] 按条件删除
来源：http://czn.hongshengwenyu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hhi.shanyushiyangkeji.top

[Q54] 清空表
来源：http://zbs.smart0.xyz

TRUNCATE TABLE logs;
来源：http://ktc.fanxiaobao.xyz

[Q55] 排名（并列占位）
来源：http://wxt.gotoacloud.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://osd.bjfxy.top

[Q56] 密集排名（并列不占位）
来源：http://mtf.snrcjt.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hxr.gzhubu.top

[Q57] 行号
来源：http://ojl.tian-w.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lwd.pycfn.com

[Q58] 累计求和
来源：http://avn.yueranfly.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hfz.gzhubu.top

[Q59] 分组内累计
来源：http://nzk.jinghuilouyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qke.tanke756.top

[Q60] 取上一行 / 下一行
来源：http://kqs.hnqzz.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://twa.zhiwuduotai.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://usn.shangyingyoupin.top

[Q61] 移动平均
来源：http://alo.daxiang520.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ixi.xuetiantiany.cn

[Q62] 分组占比
来源：http://upl.cheryme.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://khb.ybcxt.top

[Q63] 开启事务
来源：http://moj.aizwys.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kax.nanxinkj.top

[Q64] 提交事务
来源：http://qnj.zhoulong.xyz

COMMIT;
来源：http://prm.chenzaomai.com

[Q65] 回滚事务
来源：http://wge.cdnleiting.top

ROLLBACK;
来源：http://inf.xuetiantiany.cn

[Q66] 行锁查询
来源：http://ozf.sxryk.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ton.zdqjudy.top

[Q67] 设置隔离级别
来源：http://khz.xinyue.icu

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jwa.sweek.top

[Q68] 保存点
来源：http://jxh.cucudq.cn

SAVEPOINT sp1;
来源：http://paj.nanxuanxn.top

ROLLBACK TO sp1;
来源：http://zso.sufxvd.cn

[Q69] 查看执行计划
来源：http://pix.yj20258888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bmr.jinyuanbaomall.cn

[Q70] 更新统计信息
来源：http://vfg.aizwys.cn

ANALYZE TABLE users;
来源：http://vyz.guannengcc.top

[Q71] 查看建表语句
来源：http://ygu.hywenlv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wqd.fktsv.cn

[Q72] 查看索引
来源：http://nbz.shangyingyoupin.top

SHOW INDEX FROM users;
来源：http://hcs.316326.xyz

[Q73] 查看表状态
来源：http://ojx.epnwcf.com

SHOW TABLE STATUS LIKE 'users';
来源：http://dfo.zhoulong.xyz

[Q74] 强制使用索引
来源：http://hka.hnqzz.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://clo.jinghuilouyu.cn

[Q75] 日期格式化
来源：http://rqu.svipenyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kcx.xinyue.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pyy.bjfxy.top

[Q76] 按天统计
来源：http://ver.shuidangran.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kyu.fzhhl.top

[Q77] 时间加减
来源：http://xsw.dashuyun.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pai.zdqjudy.top

[Q78] 当前时间
来源：http://cza.dashuyun.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rxd.wangshuangyany.cn

[Q79] 字符串拼接
来源：http://iua.yj20258888.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://urr.feifeiyinyue.top

[Q80] 字符串截取
来源：http://ygn.chenjidiqi.icu

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ozv.xylfe.cn

[Q81] 字符串替换
来源：http://zjt.ywan-chungtsiang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nxv.chenlongwang.top

[Q82] 字符长度与字节长度
来源：http://svk.c1oappe.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://iuc.yuanzhike.top

[Q83] 大小写转换
来源：http://qyq.yongpay.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fca.fktsv.cn

[Q84] 去除首尾空格
来源：http://dna.chenjidiqi.icu

SELECT TRIM(name) FROM users;
来源：http://dzo.ywan-chungtsiang.top

[Q85] 数值取整
来源：http://utj.cashguo.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dqa.sxryk.cn

[Q86] 读取 JSON 字段
来源：http://aek.ydzc1.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ymc.tanke756.top

[Q87] JSON 字段做条件
来源：http://mhd.jinghuilouyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://epg.vqdsnc.cn

[Q88] 行转列（条件聚合）
来源：http://rlw.zycfv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wdr.fehbvm.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kso.yj20258.top

[Q89] 判断表是否存在
来源：http://xlu.dashuyun.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qnk.yuxming.cn

[Q90] 生成序号列
来源：http://puk.hysaishi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gqd.cheryme.top

================================================================================
来源：http://qqr.dashuyun.cn

R. Bash 专题
来源：http://xdc.cashguo.top

================================================================================
来源：http://rnh.yangfankeji.com

[R01] shebang 与严格模式
来源：http://qfm.xuetiantiany.cn

#!/usr/bin/env bash
来源：http://qho.smart0.xyz

set -euo pipefail
来源：http://xqp.ydjk.org.cn

[R02] 变量赋值与使用
来源：http://lqk.shanyushiyangkeji.top

name="Tom"; echo "$name"
来源：http://juj.shuidangran.top

[R03] 只读变量
来源：http://odz.sxryk.cn

readonly PI=3.14
来源：http://zfp.jyoumei.cn

[R04] 位置参数
来源：http://osq.zhixingplan.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hom.jlsjyb.cn

[R05] 参数默认值
来源：http://etm.yueranfly.top

name="${1:-default}"
来源：http://hgl.yuanzhike.top

[R06] 判断命令是否存在
来源：http://bhv.zdqjudy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hhm.316326.xyz

[R07] if 判断文件
来源：http://cwl.chenlongwang.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qck.jianghu66.top

[R08] 数值比较
来源：http://shp.chenjidiqi.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://zym.fanxiaobao.xyz

[R09] 字符串比较
来源：http://ycj.yangfankeji.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vlk.chenzaomai.com

[R10] 正则匹配
来源：http://pop.vehdjk.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zlu.yanxiufei.cn

[R11] case 多分支
来源：http://oyq.ybcxt.top

case "$1" in
来源：http://rcb.cdnleiting.top

start) echo "启动" ;;
来源：http://nmg.yj202588.top

stop)  echo "停止" ;;
来源：http://vcq.xuanzx.com

*)     echo "未知命令" ;;
来源：http://eax.svipenyu.cn

esac
来源：http://ngp.hfpthk.cn

[R12] for 遍历文件
来源：http://zbg.ppjwa.cn

for f in *.txt; do echo "$f"; done
来源：http://fyp.hnxiangtu.top

[R13] for 计数循环
来源：http://qde.aibaodan.cn

for i in {1..10}; do echo "$i"; done
来源：http://oly.sjlbkw.cn

[R14] C 风格 for
来源：http://pyd.hfpthk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ltv.xziqi.cn

[R15] while 逐行读文件
来源：http://omn.uphjek.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zpq.yangfankeji.com

[R16] until 等待条件
来源：http://iqt.andypj.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mkz.wangshuangyany.cn

[R17] 数组定义与取值
来源：http://snu.tanke756.top

arr=(a b c); echo "${arr[0]}"
来源：http://rjr.yfazqb.com

[R18] 遍历数组
来源：http://dfn.yvedp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ezr.jqgfzy.top

[R19] 数组长度
来源：http://oqf.xuanzx.com

echo "${#arr[@]}"
来源：http://uhk.hcnkem.com

[R20] 关联数组（字典）
来源：http://qyu.gaohongyu789.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dhz.haohaochexian.top

[R21] 字符串长度
来源：http://wgn.fehbvm.com

echo "${#s}"
来源：http://vpb.hesvh.cn

[R22] 截取子串
来源：http://bwx.zhongyouzk.top

echo "${s:0:5}"
来源：http://frs.fktsv.cn

[R23] 字符串替换
来源：http://cou.zhixingplan.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://otl.xziqi.cn

[R24] 大小写转换
来源：http://tbr.zhoulong.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://etq.sweek.top

[R25] 去后缀 / 去前缀
来源：http://hab.hnqzz.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dme.xylfe.cn

[R26] 命令替换
来源：http://djb.yj20258888.top

now=$(date +%F); echo "$now"
来源：http://vub.zhoulong.xyz

[R27] 算术展开
来源：http://lci.bjfxy.top

echo $((1 + 2 * 3))
来源：http://pce.52xcode.cn

[R28] 浮点运算
来源：http://kco.yuanzhike.top

echo "scale=2; 10/3" | bc
来源：http://nym.hysaishi.cn

[R29] 定义函数
来源：http://iyd.9152youxi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bhe.zhongyouzk.top

[R30] 函数返回状态码
来源：http://lqi.uphjek.com

f() { return 0; }; f || echo "失败了"
来源：http://kwf.yuxming.cn

[R31] 局部变量
来源：http://lra.cashguo.top

f() { local x=1; echo "$x"; }
来源：http://coe.shanyushiyangkeji.top

[R32] 参数个数校验
来源：http://qza.yonumen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xgz.jinqigfzy.top

[R33] 捕获错误并提示行号
来源：http://szi.sxryk.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uok.shangyingyoupin.top

[R34] 退出时清理
来源：http://fif.wangdashe.top

trap 'rm -f "$tmp"' EXIT
来源：http://jng.tanke756.top

[R35] 后台执行并等待
来源：http://lvu.guannengcc.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hvd.9152youxi.cn

[R36] 并发执行多个任务
来源：http://izm.ivvv.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tjt.xylfe.cn

[R37] 把输出赋给变量
来源：http://mya.xuanzx.com

files=$(ls -1)
来源：http://dvj.jinqigufen.top

[R38] 管道串联
来源：http://mbj.zdbjq.cn

cat a.txt | grep -i error | wc -l
来源：http://cnl.zycfv.cn

[R39] 重定向标准输出与错误
来源：http://lzs.haohaochexian.top

cmd > out.log 2>&1
来源：http://btn.yj20258.top

[R40] 追加写日志
来源：http://wps.dianchejie.cn

echo "log" >> out.log
来源：http://lym.svipenyu.cn

[R41] 丢弃输出
来源：http://tsh.aizwys.cn

cmd >/dev/null 2>&1
来源：http://cbe.ehwqpu.com

[R42] 输入重定向
来源：http://uav.andypj.xyz

wc -l < a.txt
来源：http://yiu.kuanghao11.cn

[R43] 按名字查找文件
来源：http://zoz.ehwqpu.com

find . -name "*.log" -type f
来源：http://xhc.0kj1m.cn

[R44] 按修改时间查找
来源：http://jli.shangyingyoupin.top

find . -mtime -7 -type f
来源：http://sjd.fanxiaobao.xyz

[R45] 批量删除
来源：http://tdi.haohaochexian.top

find . -name "*.tmp" -delete
来源：http://hym.redwolf501.top

[R46] 递归替换文件内容
来源：http://tgy.fzhhl.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mlf.epnwcf.com

[R47] sed 单行替换
来源：http://arj.havefunace.top

sed -i 's/foo/bar/g' a.txt
来源：http://mup.kuanghao11.cn

[R48] awk 取指定列
来源：http://jtc.shangyingyoupin.top

awk '{print $1, $3}' a.txt
来源：http://fdk.yj202588.top

[R49] awk 带条件
来源：http://ttt.jinghuilouyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mgl.ywan-chungtsiang.top

[R50] awk 求和
来源：http://mxt.shzxlz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://izw.bbcook.cn

[R51] 排序去重取前几
来源：http://vgc.epnwcf.com

sort a.txt | uniq -c | sort -rn | head
来源：http://ezd.yj20258.top

[R52] 统计行数
来源：http://awc.sjlbkw.cn

wc -l a.txt
来源：http://yxp.kuanghao11.cn

[R53] 查看文件头与实时尾
来源：http://cpe.quarkkingdee.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://whc.yueranfly.top

[R54] 比较两个文件
来源：http://qnu.bjfxy.top

diff a.txt b.txt
来源：http://oin.hysaishi.cn

[R55] 压缩与解压
来源：http://nyq.mhx1999.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://anq.shanyushiyangkeji.top

[R56] 远程拷贝
来源：http://zun.yongpay.top

scp file user@host:/path/
来源：http://mkt.shzxlz.cn

[R57] 远程执行命令
来源：http://joh.gogol.net.cn

ssh user@host 'uptime'
来源：http://enc.chenlongwang.top

[R58] 下载文件
来源：http://rno.nanxinkj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hpj.ydzc1.top

[R59] 发 POST JSON
来源：http://pbm.ywan-chungtsiang.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qsg.fanxiaobao.xyz

[R60] 只看 HTTP 状态码
来源：http://svr.yj20258.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iyp.daria6918.cn

[R61] 磁盘占用
来源：http://rip.zdqjudy.top

df -h;  du -sh *
来源：http://xvn.sxryk.cn

[R62] 找最占空间的文件
来源：http://vcq.sysykeji.top

du -ah . | sort -rh | head -10
来源：http://tly.pycfn.com

[R63] 内存与进程
来源：http://vve.hammf.cn

free -h;  ps aux | grep nginx
来源：http://tyq.ctjpmb.com

[R64] 结束进程
来源：http://col.shzxlz.cn

kill -9 $(pgrep -f app.py)
来源：http://ilv.bbcook.cn

[R65] 查看端口占用
来源：http://sen.gogol.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://are.sufxvd.cn

[R66] 定时任务
来源：http://gfl.aizwys.cn

crontab -e;  crontab -l
来源：http://sti.shangyingyoupin.top

[R67] 生成随机十六进制串
来源：http://zum.guannengcc.top

openssl rand -hex 16
来源：http://rop.tanke756.top

[R68] 计算文件校验值
来源：http://swg.hammf.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mpt.ybcxt.top

[R69] 生成随机密码
来源：http://ayj.gogol.net.cn

head -c 16 /dev/urandom | base64
来源：http://wap.ctjpmb.com

[R70] 时间戳与互转
来源：http://eak.gotoacloud.top

date +%s;  date -d @1700000000
来源：http://dfx.cdnleiting.top

[R71] 日期格式化
来源：http://iic.cqqwz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xbg.cheryme.top

[R72] 等待端口就绪
来源：http://mbn.hnqzz.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rlp.yj20258888.top

[R73] 分割大日志
来源：http://nbx.xylfe.cn

split -l 1000 big.log part_
来源：http://dxr.9152youxi.cn

[R74] 批量重命名
来源：http://wan.jianghu66.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fix.pengpengdd.cyou

[R75] 导出环境变量
来源：http://fqh.zhengqikj.top


<!-- 参考信息 -->