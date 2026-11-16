代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cym.gaohongyu789.top

[Q28] 求和与平均
来源：http://kfo.vqdsnc.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dcv.gogol.net.cn

[Q29] 最大最小值
来源：http://stl.yj202588.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://hun.wangdashe.top

[Q30] 分组统计
来源：http://uio.yvedp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://iyf.316326.xyz

[Q31] 分组后过滤
来源：http://hmh.bjfxy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ngr.yonumen.top

[Q32] 分组拼接字符串
来源：http://vmg.shangyingyoupin.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://utu.fehbvm.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wpr.shzxlz.cn

[Q33] 多列分组
来源：http://nml.jlsjyb.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gwb.xylfe.cn

[Q34] 每组取第一条
来源：http://uuk.daxiang520.top

SELECT * FROM (
来源：http://adc.wangshuangyany.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nax.hcnkem.com

) t WHERE rn = 1;
来源：http://ioh.wangdashe.top

[Q35] 内连接
来源：http://vpc.hcnkem.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fxx.jinqigfzy.top

[Q36] 左连接
来源：http://kqi.quarkkingdee.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zog.ehwqpu.com

[Q37] 右连接
来源：http://nso.zhijiandao.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://doc.ivvv.top

[Q38] 全外连接（PostgreSQL）
来源：http://uxp.ywan-chungtsiang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pil.zhengqikj.top

[Q39] 自连接（查上下级）
来源：http://phc.gogol.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://njp.ywan-chungtsiang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://srj.xuetiantiany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tok.pycfn.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rzc.xingfuxueyuan.xyz

[Q41] 多表连接
来源：http://ery.xziqi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uar.daria6918.cn

JOIN users u ON u.id = o.user_id
来源：http://gzi.yueranfly.top

JOIN products p ON p.id = o.product_id;
来源：http://qjy.yueranfly.top

[Q42] 连接条件附加过滤
来源：http://ilf.c1oappe.top

SELECT u.name, o.amount FROM users u
来源：http://ppa.xuetiantiany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://izu.iojbl.cn

[Q43] 标量子查询
来源：http://lhw.kuanghao11.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gln.zhiwuduotai.top

[Q44] IN 子查询
来源：http://jep.vqdsnc.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mzr.gaohongyu789.top

[Q45] EXISTS 判断存在
来源：http://cfv.uphjek.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dsd.jinyuanbaomall.cn

[Q46] NOT EXISTS 判断不存在
来源：http://goq.ctjpmb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nsr.kuanghao11.cn

[Q47] 与平均值比较
来源：http://akc.c1oappe.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gfs.zycfv.cn

[Q48] CTE 公用表表达式
来源：http://jbj.jqgufenzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://int.fktsv.cn

SELECT * FROM t WHERE c > 5;
来源：http://wvf.vehdjk.com

[Q49] 更新单行
来源：http://bca.jianghu66.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pgz.jinqigfzy.top

[Q50] 批量更新
来源：http://cyi.hammf.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://day.meibo888.top

[Q51] 用子查询更新
来源：http://dxj.hongshengwenyu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cpw.guowangkeji.top

[Q52] 删除指定行
来源：http://vik.jinqigfzy.top

DELETE FROM users WHERE id = 10;
来源：http://nza.yvedp.cn

[Q53] 按条件删除
来源：http://xgu.zhengqikj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qmz.jinyuanbaomall.cn

[Q54] 清空表
来源：http://owq.zhengqikj.top

TRUNCATE TABLE logs;
来源：http://xtp.redwolf501.top

[Q55] 排名（并列占位）
来源：http://rdr.yfazqb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zup.ctjpmb.com

[Q56] 密集排名（并列不占位）
来源：http://knk.tian-w.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bqy.epnwcf.com

[Q57] 行号
来源：http://xat.bjfxy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lip.fktsv.cn

[Q58] 累计求和
来源：http://pje.wangshuangyany.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yzn.sysykeji.top

[Q59] 分组内累计
来源：http://zwd.jlsjyb.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rrn.haohaochexian.top

[Q60] 取上一行 / 下一行
来源：http://cgh.mhx1999.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://inc.vehdjk.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vzf.yvedp.cn

[Q61] 移动平均
来源：http://lws.sjlbkw.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://few.cdnleiting.top

[Q62] 分组占比
来源：http://eyv.fanxiaobao.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fky.zhixingplan.top

[Q63] 开启事务
来源：http://xwa.bjfxy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://okp.tian-w.cn

[Q64] 提交事务
来源：http://xlj.meibo888.top

COMMIT;
来源：http://poy.yueranfly.top

[Q65] 回滚事务
来源：http://cmy.xziqi.cn

ROLLBACK;
来源：http://xqc.pengpengdd.cyou

[Q66] 行锁查询
来源：http://ijr.fktsv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ihx.zdqjudy.top

[Q67] 设置隔离级别
来源：http://xup.cqqwz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kif.yj202588.top

[Q68] 保存点
来源：http://ehj.zhiwuduotai.top

SAVEPOINT sp1;
来源：http://bfw.aizwys.cn

ROLLBACK TO sp1;
来源：http://cbm.fzhhl.top

[Q69] 查看执行计划
来源：http://fal.quarkkingdee.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zqk.fzhhl.top

[Q70] 更新统计信息
来源：http://hng.yuxming.cn

ANALYZE TABLE users;
来源：http://qhy.tian-w.cn

[Q71] 查看建表语句
来源：http://voa.haohaochexian.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cbk.gaohongyu789.top

[Q72] 查看索引
来源：http://hdi.jinqigufen.top

SHOW INDEX FROM users;
来源：http://gft.havefunace.top

[Q73] 查看表状态
来源：http://nkn.sweek.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ugs.gogol.net.cn

[Q74] 强制使用索引
来源：http://qtz.nwbrower.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tuu.nwbrower.top

[Q75] 日期格式化
来源：http://los.andypj.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://phk.0kj1m.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vfr.shanyushiyangkeji.top

[Q76] 按天统计
来源：http://zmq.xinyue.icu

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://utf.ehwqpu.com

[Q77] 时间加减
来源：http://oaa.zhoulong.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xmt.gotoacloud.top

[Q78] 当前时间
来源：http://wkw.xuanzx.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ebu.gogol.net.cn

[Q79] 字符串拼接
来源：http://cvf.daxiang520.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://foi.aibaodan.cn

[Q80] 字符串截取
来源：http://uxo.sweek.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fjw.dashuyun.cn

[Q81] 字符串替换
来源：http://iow.xingfuxueyuan.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://unw.hnxiangtu.top

[Q82] 字符长度与字节长度
来源：http://jkd.gaohongyu789.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cnn.52xcode.cn

[Q83] 大小写转换
来源：http://jvg.zdqjudy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bus.hysaishi.cn

[Q84] 去除首尾空格
来源：http://lvo.fzhhl.top

SELECT TRIM(name) FROM users;
来源：http://uat.sxryk.cn

[Q85] 数值取整
来源：http://inx.xinyue.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cfu.hysaishi.cn

[Q86] 读取 JSON 字段
来源：http://yyn.yangfankeji.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xkg.zdqjudy.top

[Q87] JSON 字段做条件
来源：http://wdw.fktsv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ddw.gogol.net.cn

[Q88] 行转列（条件聚合）
来源：http://huj.dianchejie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dyq.dashuyun.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pea.tanke756.top

[Q89] 判断表是否存在
来源：http://jax.quarkkingdee.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://iex.chenzaomai.com

[Q90] 生成序号列
来源：http://cet.yvedp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ube.hnqzz.top

================================================================================
来源：http://vvv.ppjwa.cn

R. Bash 专题
来源：http://otc.fehbvm.com

================================================================================
来源：http://nwo.sysykeji.top

[R01] shebang 与严格模式
来源：http://nhj.havefunace.top

#!/usr/bin/env bash
来源：http://lsr.jqgfzy.top

set -euo pipefail
来源：http://hct.sweek.top

[R02] 变量赋值与使用
来源：http://clq.hywenlv.cn

name="Tom"; echo "$name"
来源：http://kdz.yuanzhike.top

[R03] 只读变量
来源：http://lvd.bjfxy.top

readonly PI=3.14
来源：http://oou.dianchejie.cn

[R04] 位置参数
来源：http://zgk.wangshuangyany.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://crf.tanke756.top

[R05] 参数默认值
来源：http://wcu.epnwcf.com

name="${1:-default}"
来源：http://dgy.cheryme.top

[R06] 判断命令是否存在
来源：http://pwb.sysykeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vtx.fehbvm.com

[R07] if 判断文件
来源：http://vvk.sufxvd.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wuq.wangdashe.top

[R08] 数值比较
来源：http://avc.cqqwz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://znw.hysaishi.cn

[R09] 字符串比较
来源：http://pzr.ydjk.org.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uee.yongpay.top

[R10] 正则匹配
来源：http://wmo.yfazqb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yph.xuetiantiany.cn

[R11] case 多分支
来源：http://gum.uphjek.com

case "$1" in
来源：http://tts.yongpay.top

start) echo "启动" ;;
来源：http://chj.jinqigufen.top

stop)  echo "停止" ;;
来源：http://oxa.xylfe.cn

*)     echo "未知命令" ;;
来源：http://bpj.sxryk.cn

esac
来源：http://ulj.yongpay.top

[R12] for 遍历文件
来源：http://tsk.vehdjk.com

for f in *.txt; do echo "$f"; done
来源：http://bdh.shangyingyoupin.top

[R13] for 计数循环
来源：http://fby.hcnkem.com

for i in {1..10}; do echo "$i"; done
来源：http://dwz.jianghu66.top

[R14] C 风格 for
来源：http://yql.daria6918.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://agt.tian-w.cn

[R15] while 逐行读文件
来源：http://lbz.hywenlv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jdr.shanyushiyangkeji.top

[R16] until 等待条件
来源：http://qlm.jqgfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lpv.dianchejie.cn

[R17] 数组定义与取值
来源：http://cou.jinqigufen.top

arr=(a b c); echo "${arr[0]}"
来源：http://iro.fzhhl.top

[R18] 遍历数组
来源：http://xag.yuanzhike.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rki.sysykeji.top

[R19] 数组长度
来源：http://ars.cdnleiting.top

echo "${#arr[@]}"
来源：http://mhk.hnqzz.top

[R20] 关联数组（字典）
来源：http://tje.0kj1m.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ovs.jinqigfzy.top

[R21] 字符串长度
来源：http://bnf.ywan-chungtsiang.top

echo "${#s}"
来源：http://bmr.fanxiaobao.xyz

[R22] 截取子串
来源：http://zqi.haohaochexian.top

echo "${s:0:5}"
来源：http://fqj.zycfv.cn

[R23] 字符串替换
来源：http://szw.xinyue.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fem.yvedp.cn

[R24] 大小写转换
来源：http://ndl.yj20258.top

echo "${s^^}"; echo "${s,,}"
来源：http://njh.daxiang520.top

[R25] 去后缀 / 去前缀
来源：http://slv.havefunace.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zoa.sxryk.cn

[R26] 命令替换
来源：http://nco.ybcxt.top

now=$(date +%F); echo "$now"
来源：http://bjo.xinyue.icu

[R27] 算术展开
来源：http://rnq.shzxlz.cn

echo $((1 + 2 * 3))
来源：http://lbk.zdqjudy.top

[R28] 浮点运算
来源：http://cxg.mhx1999.top

echo "scale=2; 10/3" | bc
来源：http://rnr.shanyushiyangkeji.top

[R29] 定义函数
来源：http://bcu.yonumen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bzr.haohaochexian.top

[R30] 函数返回状态码
来源：http://fbk.yuanzhike.top

f() { return 0; }; f || echo "失败了"
来源：http://bzs.fzhhl.top

[R31] 局部变量
来源：http://qky.ehwqpu.com

f() { local x=1; echo "$x"; }
来源：http://jlm.bbcook.cn

[R32] 参数个数校验
来源：http://hgq.aibaodan.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://acw.fanxiaobao.xyz

[R33] 捕获错误并提示行号
来源：http://lea.fehbvm.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qkb.tanke756.top

[R34] 退出时清理
来源：http://rtb.hammf.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wjn.zhoulong.xyz

[R35] 后台执行并等待
来源：http://dfg.vehdjk.com

sleep 5 & pid=$!; wait "$pid"
来源：http://jcs.jlsjyb.cn

[R36] 并发执行多个任务
来源：http://nrl.guowangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://joj.nwbrower.top

[R37] 把输出赋给变量
来源：http://opo.fengsongda.top

files=$(ls -1)
来源：http://xgv.jyoumei.cn

[R38] 管道串联
来源：http://ixy.fehbvm.com

cat a.txt | grep -i error | wc -l
来源：http://kod.jiagoushi.top

[R39] 重定向标准输出与错误
来源：http://rbu.chenzaomai.com

cmd > out.log 2>&1
来源：http://zis.ywan-chungtsiang.top

[R40] 追加写日志
来源：http://ofl.xinyue.icu

echo "log" >> out.log
来源：http://uun.xuanzx.com

[R41] 丢弃输出
来源：http://qle.havefunace.top

cmd >/dev/null 2>&1
来源：http://kka.chenlongwang.top

[R42] 输入重定向
来源：http://dmd.ydzc1.top

wc -l < a.txt
来源：http://jjf.jqgufenzy.top

[R43] 按名字查找文件
来源：http://cem.ywan-chungtsiang.top

find . -name "*.log" -type f
来源：http://aht.snrcjt.cn

[R44] 按修改时间查找
来源：http://vcn.fanxiaobao.xyz

find . -mtime -7 -type f
来源：http://ssb.aibaodan.cn

[R45] 批量删除
来源：http://nmf.jianghu66.top

find . -name "*.tmp" -delete
来源：http://buy.nanxuanxn.top

[R46] 递归替换文件内容
来源：http://bws.zhixingplan.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ihe.hammf.cn

[R47] sed 单行替换
来源：http://rdi.zhixingplan.top

sed -i 's/foo/bar/g' a.txt
来源：http://wbq.wangshuangyany.cn

[R48] awk 取指定列
来源：http://gbg.wangshuangyany.cn

awk '{print $1, $3}' a.txt
来源：http://jvz.jiagoushi.top

[R49] awk 带条件
来源：http://ban.sysykeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ibv.guannengcc.top

[R50] awk 求和
来源：http://vaq.zhijiandao.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yhf.svipenyu.cn

[R51] 排序去重取前几
来源：http://qji.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zlm.havefunace.top

[R52] 统计行数
来源：http://qjh.smart0.xyz

wc -l a.txt
来源：http://jdx.yvedp.cn

[R53] 查看文件头与实时尾
来源：http://qec.birdmap.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rhs.shzxlz.cn

[R54] 比较两个文件
来源：http://jyp.ppjwa.cn

diff a.txt b.txt
来源：http://vam.zdqjudy.top

[R55] 压缩与解压
来源：http://bfz.daria6918.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gkt.wangshuangyany.cn

[R56] 远程拷贝
来源：http://txf.yangfankeji.com

scp file user@host:/path/
来源：http://vvy.xingfuxueyuan.xyz

[R57] 远程执行命令
来源：http://mvb.sufxvd.cn

ssh user@host 'uptime'
来源：http://qxu.zycfv.cn

[R58] 下载文件
来源：http://uxv.hywenlv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://aav.havefunace.top

[R59] 发 POST JSON
来源：http://tcm.xuanzx.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gzm.jlsjyb.cn

[R60] 只看 HTTP 状态码
来源：http://yoh.gotoacloud.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dng.cheryme.top

[R61] 磁盘占用
来源：http://scu.cqqwz.cn

df -h;  du -sh *
来源：http://upv.pycfn.com

[R62] 找最占空间的文件
来源：http://lcb.iojbl.cn

du -ah . | sort -rh | head -10
来源：http://bkh.gaohongyu789.top

[R63] 内存与进程
来源：http://bkv.svipenyu.cn

free -h;  ps aux | grep nginx
来源：http://bsf.hywenlv.cn

[R64] 结束进程
来源：http://jwr.zhongyouzk.top

kill -9 $(pgrep -f app.py)
来源：http://ghf.sufxvd.cn

[R65] 查看端口占用
来源：http://xim.vqdsnc.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nma.andypj.xyz

[R66] 定时任务
来源：http://hnu.fehbvm.com

crontab -e;  crontab -l
来源：http://nry.xuanzx.com

[R67] 生成随机十六进制串
来源：http://gnh.pengpengdd.cyou

openssl rand -hex 16
来源：http://pxf.tarul.cn

[R68] 计算文件校验值
来源：http://kue.nanxuanxn.top

sha256sum a.txt;  md5sum a.txt
来源：http://ugf.cdnleiting.top

[R69] 生成随机密码
来源：http://oai.sufxvd.cn

head -c 16 /dev/urandom | base64
来源：http://lzk.hnqzz.top

[R70] 时间戳与互转
来源：http://fwc.ybcxt.top

date +%s;  date -d @1700000000
来源：http://kqw.birdmap.top

[R71] 日期格式化
来源：http://jvt.yuanzhike.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zya.yonumen.top

[R72] 等待端口就绪
来源：http://cwd.birdmap.top

until nc -z localhost 3306; do sleep 1; done
来源：http://epy.ivvv.top

[R73] 分割大日志
来源：http://iof.zhoulong.xyz

split -l 1000 big.log part_
来源：http://pkz.pengpengdd.cyou

[R74] 批量重命名
来源：http://uea.yj20258888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vfq.aibaodan.cn

[R75] 导出环境变量
来源：http://iky.kuanghao11.cn

export PATH="$HOME/bin:$PATH"
来源：http://npg.xylfe.cn

[R76] 使用临时文件
来源：http://kab.vehdjk.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mov.pengpengdd.cyou

[R77] 读取用户输入
来源：http://tqp.epnwcf.com


<!-- 参考信息 -->