代发 wailian999

SELECT * FROM users;
来源：http://tvh.shuidangran.top

[Q16] 查询指定列
来源：http://ozv.xingfuxueyuan.xyz

SELECT id, name FROM users;
来源：http://isb.nanxinkj.top

[Q17] 条件查询
来源：http://zgr.nanxuanxn.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://szm.cqqwz.cn

[Q18] 模糊匹配
来源：http://muu.nanxinkj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://txg.yj20258888.top

[Q19] 范围查询
来源：http://zmv.tian-w.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mtl.meibo888.top

[Q20] IN 列表
来源：http://jix.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pqn.epnwcf.com

[Q21] 空值判断
来源：http://ani.vqdsnc.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wyq.xuanzx.com

[Q22] 排序
来源：http://fyv.yongpay.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jny.daria6918.cn

[Q23] 分页
来源：http://ibe.jlsjyb.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vlr.sweek.top

[Q24] 去重
来源：http://ael.jinghuilouyu.cn

SELECT DISTINCT city FROM users;
来源：http://qwy.zhaomingkeji.xyz

[Q25] 只取前 N 条
来源：http://nmt.nanxuanxn.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hej.xuetiantiany.cn

[Q26] 计数
来源：http://fub.wangshuangyany.cn

SELECT COUNT(*) FROM users;
来源：http://ezf.nanxinkj.top

[Q27] 条件计数
来源：http://uxw.xinyue.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tlc.fzhhl.top

[Q28] 求和与平均
来源：http://pkn.chenjidiqi.icu

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hob.sjlbkw.cn

[Q29] 最大最小值
来源：http://lym.bbcook.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jlu.ybcxt.top

[Q30] 分组统计
来源：http://gdn.zhongyouzk.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eby.zhongyouzk.top

[Q31] 分组后过滤
来源：http://nkz.xuetiantiany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qku.kuanghao11.cn

[Q32] 分组拼接字符串
来源：http://xjc.fehbvm.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://orr.havefunace.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tyx.sxryk.cn

[Q33] 多列分组
来源：http://wow.xinyue.icu

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://epo.zhijiandao.cn

[Q34] 每组取第一条
来源：http://bam.nanxuanxn.top

SELECT * FROM (
来源：http://mdd.sysykeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jzv.yuanzhike.top

) t WHERE rn = 1;
来源：http://wdv.jianghu66.top

[Q35] 内连接
来源：http://cpn.fktsv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gsu.hfpthk.cn

[Q36] 左连接
来源：http://miq.iojbl.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bvo.chenjidiqi.icu

[Q37] 右连接
来源：http://mec.zycfv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://byb.shzxlz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://uiv.ydzc1.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dfs.shangyingyoupin.top

[Q39] 自连接（查上下级）
来源：http://ghu.smart0.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://yzx.sufxvd.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vem.chenlongwang.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wuw.ppjwa.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wzv.jinqigufen.top

[Q41] 多表连接
来源：http://gwv.wangshuangyany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://usr.xylfe.cn

JOIN users u ON u.id = o.user_id
来源：http://bdw.ydzc1.top

JOIN products p ON p.id = o.product_id;
来源：http://eah.zhengqikj.top

[Q42] 连接条件附加过滤
来源：http://tdh.cashguo.top

SELECT u.name, o.amount FROM users u
来源：http://kgf.zdqjudy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nzp.fzhhl.top

[Q43] 标量子查询
来源：http://dxa.c1oappe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jxq.ydzc1.top

[Q44] IN 子查询
来源：http://jec.shangyingyoupin.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zaf.vehdjk.com

[Q45] EXISTS 判断存在
来源：http://kao.hongshengwenyu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zpg.fanxiaobao.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://wbj.hesvh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hso.0kj1m.cn

[Q47] 与平均值比较
来源：http://ila.hywenlv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zwk.shuidangran.top

[Q48] CTE 公用表表达式
来源：http://ehw.yueranfly.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vqs.fehbvm.com

SELECT * FROM t WHERE c > 5;
来源：http://zdx.jinqigufen.top

[Q49] 更新单行
来源：http://qlt.fengsongda.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fiq.yongpay.top

[Q50] 批量更新
来源：http://vng.dashuyun.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dwa.wangshuangyany.cn

[Q51] 用子查询更新
来源：http://inr.9152youxi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tcq.dianchejie.cn

[Q52] 删除指定行
来源：http://yea.uphjek.com

DELETE FROM users WHERE id = 10;
来源：http://csm.sysykeji.top

[Q53] 按条件删除
来源：http://pyz.yj202588.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rot.zhiwuduotai.top

[Q54] 清空表
来源：http://ryw.zhoulong.xyz

TRUNCATE TABLE logs;
来源：http://wbc.guannengcc.top

[Q55] 排名（并列占位）
来源：http://xeb.ctjpmb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pcj.aibaodan.cn

[Q56] 密集排名（并列不占位）
来源：http://kwv.shanyushiyangkeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lqz.shzxlz.cn

[Q57] 行号
来源：http://wjy.fengsongda.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tum.hesvh.cn

[Q58] 累计求和
来源：http://wxk.aibaodan.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zut.redwolf501.top

[Q59] 分组内累计
来源：http://vdz.gogol.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ycn.yfazqb.com

[Q60] 取上一行 / 下一行
来源：http://drs.kuanghao11.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ogc.hnqzz.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hbo.yj202588.top

[Q61] 移动平均
来源：http://yrx.52xcode.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vie.xingfuxueyuan.xyz

[Q62] 分组占比
来源：http://soj.52xcode.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ybp.shzxlz.cn

[Q63] 开启事务
来源：http://don.yanxiufei.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dvb.kuanghao11.cn

[Q64] 提交事务
来源：http://eew.zycfv.cn

COMMIT;
来源：http://xqu.cqqwz.cn

[Q65] 回滚事务
来源：http://ikd.zhengqikj.top

ROLLBACK;
来源：http://znw.sufxvd.cn

[Q66] 行锁查询
来源：http://vzg.zhijiandao.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bqq.kuanghao11.cn

[Q67] 设置隔离级别
来源：http://tdm.nanxinkj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://htd.chenjidiqi.icu

[Q68] 保存点
来源：http://axb.yj20258888.top

SAVEPOINT sp1;
来源：http://nyt.gaohongyu789.top

ROLLBACK TO sp1;
来源：http://blw.yonumen.top

[Q69] 查看执行计划
来源：http://lgo.fzhhl.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oqr.bjfxy.top

[Q70] 更新统计信息
来源：http://cte.hnqzz.top

ANALYZE TABLE users;
来源：http://xhr.shangyingyoupin.top

[Q71] 查看建表语句
来源：http://coh.xziqi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vzf.jlsjyb.cn

[Q72] 查看索引
来源：http://tjo.chenjidiqi.icu

SHOW INDEX FROM users;
来源：http://kmy.jqgfzy.top

[Q73] 查看表状态
来源：http://pmt.meibo888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://trn.zdbjq.cn

[Q74] 强制使用索引
来源：http://ytq.cashguo.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xmn.ydjk.org.cn

[Q75] 日期格式化
来源：http://hzn.chenzaomai.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dev.tian-w.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dhb.wangshuangyany.cn

[Q76] 按天统计
来源：http://fmv.sysykeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ryi.sysykeji.top

[Q77] 时间加减
来源：http://fqc.daxiang520.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xud.cdnleiting.top

[Q78] 当前时间
来源：http://rlf.hesvh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qzk.guowangkeji.top

[Q79] 字符串拼接
来源：http://ndg.zhongyouzk.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kps.ybcxt.top

[Q80] 字符串截取
来源：http://sfj.yj20258.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kfo.hnqzz.top

[Q81] 字符串替换
来源：http://uyh.vehdjk.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ufr.chenzaomai.com

[Q82] 字符长度与字节长度
来源：http://jxu.aizwys.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://njp.zhixingplan.top

[Q83] 大小写转换
来源：http://frl.shzxlz.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yaz.jlsjyb.cn

[Q84] 去除首尾空格
来源：http://gxs.ydjk.org.cn

SELECT TRIM(name) FROM users;
来源：http://css.yfazqb.com

[Q85] 数值取整
来源：http://nhv.gogol.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xuv.quarkkingdee.top

[Q86] 读取 JSON 字段
来源：http://moo.shanyushiyangtech.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ori.jlsjyb.cn

[Q87] JSON 字段做条件
来源：http://faq.yuxming.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yjc.xuanzx.com

[Q88] 行转列（条件聚合）
来源：http://uor.nanxinkj.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://olj.pengpengdd.cyou

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tbw.yfazqb.com

[Q89] 判断表是否存在
来源：http://yqe.hnqzz.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dkb.shanyushiyangtech.top

[Q90] 生成序号列
来源：http://noa.gaohongyu789.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rip.yvedp.cn

================================================================================
来源：http://lrb.haohaochexian.top

R. Bash 专题
来源：http://nme.yongpay.top

================================================================================
来源：http://wlz.jqgfzy.top

[R01] shebang 与严格模式
来源：http://hax.hammf.cn

#!/usr/bin/env bash
来源：http://nmv.zhengqikj.top

set -euo pipefail
来源：http://wcn.hnxiangtu.top

[R02] 变量赋值与使用
来源：http://xkh.jiagoushi.top

name="Tom"; echo "$name"
来源：http://qvv.birdmap.top

[R03] 只读变量
来源：http://wrs.redwolf501.top

readonly PI=3.14
来源：http://ocj.shzxlz.cn

[R04] 位置参数
来源：http://arv.jinqigfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jmr.zycfv.cn

[R05] 参数默认值
来源：http://ncw.jinqigufen.top

name="${1:-default}"
来源：http://ygs.0kj1m.cn

[R06] 判断命令是否存在
来源：http://oyg.hnxiangtu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xep.dashuyun.cn

[R07] if 判断文件
来源：http://hsd.ivvv.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wrc.zhoulong.xyz

[R08] 数值比较
来源：http://xwk.guannengcc.top

if (( a > b )); then echo "a 更大"; fi
来源：http://oie.gotoacloud.top

[R09] 字符串比较
来源：http://ada.hywenlv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ium.zhijiandao.cn

[R10] 正则匹配
来源：http://knh.aibaodan.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ftl.yj20258888.top

[R11] case 多分支
来源：http://ply.epnwcf.com

case "$1" in
来源：http://afm.chenjidiqi.icu

start) echo "启动" ;;
来源：http://rxz.xylfe.cn

stop)  echo "停止" ;;
来源：http://cqm.ppjwa.cn

*)     echo "未知命令" ;;
来源：http://xhz.hammf.cn

esac
来源：http://dne.snrcjt.cn

[R12] for 遍历文件
来源：http://hmh.epnwcf.com

for f in *.txt; do echo "$f"; done
来源：http://fuo.hongshengwenyu.top

[R13] for 计数循环
来源：http://kor.wangshuangyany.cn

for i in {1..10}; do echo "$i"; done
来源：http://bmw.yanxiufei.cn

[R14] C 风格 for
来源：http://mkp.hcnkem.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yzn.gotoacloud.top

[R15] while 逐行读文件
来源：http://zxv.nanxuanxn.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gco.uphjek.com

[R16] until 等待条件
来源：http://mxl.mhx1999.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://czb.havefunace.top

[R17] 数组定义与取值
来源：http://pzn.ctjpmb.com

arr=(a b c); echo "${arr[0]}"
来源：http://jcn.guannengcc.top

[R18] 遍历数组
来源：http://iov.shangyingyoupin.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lsp.zhongyouzk.top

[R19] 数组长度
来源：http://ofa.cucudq.cn

echo "${#arr[@]}"
来源：http://csf.xziqi.cn

[R20] 关联数组（字典）
来源：http://pkw.zhiwuduotai.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://epq.chenjidiqi.icu

[R21] 字符串长度
来源：http://pvk.xziqi.cn

echo "${#s}"
来源：http://mxl.bbcook.cn

[R22] 截取子串
来源：http://cyj.shangyingyoupin.top

echo "${s:0:5}"
来源：http://uoa.daria6918.cn

[R23] 字符串替换
来源：http://dnh.aibaodan.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ntx.ywan-chungtsiang.top

[R24] 大小写转换
来源：http://ntn.zhengqikj.top

echo "${s^^}"; echo "${s,,}"
来源：http://dzj.hongshengwenyu.top

[R25] 去后缀 / 去前缀
来源：http://oax.yuanzhike.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://wfb.hfpthk.cn

[R26] 命令替换
来源：http://amf.yueranfly.top

now=$(date +%F); echo "$now"
来源：http://vje.cdnleiting.top

[R27] 算术展开
来源：http://xwn.snrcjt.cn

echo $((1 + 2 * 3))
来源：http://qii.hywenlv.cn

[R28] 浮点运算
来源：http://hhc.epnwcf.com

echo "scale=2; 10/3" | bc
来源：http://ycb.ctjpmb.com

[R29] 定义函数
来源：http://txm.haohaochexian.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bvo.9152youxi.cn

[R30] 函数返回状态码
来源：http://hva.ehwqpu.com

f() { return 0; }; f || echo "失败了"
来源：http://sym.zhoulong.xyz

[R31] 局部变量
来源：http://cyg.sjlbkw.cn

f() { local x=1; echo "$x"; }
来源：http://wks.yj202588.top

[R32] 参数个数校验
来源：http://afk.jinqigufen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://noi.jinqigufen.top

[R33] 捕获错误并提示行号
来源：http://rif.gotoacloud.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uqu.hnxiangtu.top

[R34] 退出时清理
来源：http://fyk.xinyue.icu

trap 'rm -f "$tmp"' EXIT
来源：http://mvd.fehbvm.com

[R35] 后台执行并等待
来源：http://rmm.yuxming.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://udd.hnxiangtu.top

[R36] 并发执行多个任务
来源：http://fpu.sxryk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://otk.mhx1999.top

[R37] 把输出赋给变量
来源：http://dls.yuxming.cn

files=$(ls -1)
来源：http://pck.ybcxt.top

[R38] 管道串联
来源：http://hux.snrcjt.cn

cat a.txt | grep -i error | wc -l
来源：http://xsr.hfpthk.cn

[R39] 重定向标准输出与错误
来源：http://iyh.gogol.net.cn

cmd > out.log 2>&1
来源：http://ejo.fengsongda.top

[R40] 追加写日志
来源：http://dft.fanxiaobao.xyz

echo "log" >> out.log
来源：http://ktb.zhiwuduotai.top

[R41] 丢弃输出
来源：http://axu.zycfv.cn

cmd >/dev/null 2>&1
来源：http://zyr.xuetiantiany.cn

[R42] 输入重定向
来源：http://ale.yangfankeji.com

wc -l < a.txt
来源：http://nsv.haohaochexian.top

[R43] 按名字查找文件
来源：http://wyr.sufxvd.cn

find . -name "*.log" -type f
来源：http://nsl.ppjwa.cn

[R44] 按修改时间查找
来源：http://sca.hysaishi.cn

find . -mtime -7 -type f
来源：http://ndp.chenjidiqi.icu

[R45] 批量删除
来源：http://rbi.9152youxi.cn

find . -name "*.tmp" -delete
来源：http://sit.gzhubu.top

[R46] 递归替换文件内容
来源：http://ijr.gogol.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://brb.sweek.top

[R47] sed 单行替换
来源：http://shp.ctjpmb.com

sed -i 's/foo/bar/g' a.txt
来源：http://ukn.chenzaomai.com

[R48] awk 取指定列
来源：http://sfl.jinqigfzy.top

awk '{print $1, $3}' a.txt
来源：http://ywj.nanxinkj.top

[R49] awk 带条件
来源：http://oam.sweek.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wxe.jinqigfzy.top

[R50] awk 求和
来源：http://fih.hesvh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://uei.svipenyu.cn

[R51] 排序去重取前几
来源：http://bji.ppjwa.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cgc.yueranfly.top

[R52] 统计行数
来源：http://hlt.ydzc1.top

wc -l a.txt
来源：http://lyz.chenzaomai.com

[R53] 查看文件头与实时尾
来源：http://aiz.nanxuanxn.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://whm.shanyushiyangkeji.top

[R54] 比较两个文件
来源：http://npi.hysaishi.cn

diff a.txt b.txt
来源：http://nnu.sweek.top

[R55] 压缩与解压
来源：http://flu.zhixingplan.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kuh.chenjidiqi.icu

[R56] 远程拷贝
来源：http://jji.smart0.xyz

scp file user@host:/path/
来源：http://qqu.fehbvm.com

[R57] 远程执行命令
来源：http://ryk.shangyingyoupin.top

ssh user@host 'uptime'
来源：http://tbh.zhongyouzk.top

[R58] 下载文件
来源：http://flx.jiagoushi.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rtb.fehbvm.com

[R59] 发 POST JSON
来源：http://tpk.chenjidiqi.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mun.pengpengdd.cyou

[R60] 只看 HTTP 状态码
来源：http://dwu.zhixingplan.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://koy.daria6918.cn

[R61] 磁盘占用
来源：http://hob.pycfn.com

df -h;  du -sh *
来源：http://nfm.yj20258888.top

[R62] 找最占空间的文件
来源：http://jwk.yangfankeji.com

du -ah . | sort -rh | head -10
来源：http://pwy.zycfv.cn

[R63] 内存与进程
来源：http://nmm.aizwys.cn

free -h;  ps aux | grep nginx
来源：http://gqi.xuanzx.com

[R64] 结束进程
来源：http://mhq.tanke756.top

kill -9 $(pgrep -f app.py)
来源：http://zqw.ywan-chungtsiang.top

[R65] 查看端口占用
来源：http://qha.316326.xyz


<!-- 参考信息 -->