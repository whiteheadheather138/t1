代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lsd.jqgfzy.top

[Q20] IN 列表
来源：http://vqw.birdmap.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gza.jyoumei.cn

[Q21] 空值判断
来源：http://bys.snrcjt.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pid.xinyue.icu

[Q22] 排序
来源：http://kmo.jinqigufen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tse.jlsjyb.cn

[Q23] 分页
来源：http://fla.cqqwz.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gel.quarkkingdee.top

[Q24] 去重
来源：http://rts.gotoacloud.top

SELECT DISTINCT city FROM users;
来源：http://qca.jqgufenzy.top

[Q25] 只取前 N 条
来源：http://ark.hfpthk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://doy.quarkkingdee.top

[Q26] 计数
来源：http://cgz.chenzaomai.com

SELECT COUNT(*) FROM users;
来源：http://esq.sxryk.cn

[Q27] 条件计数
来源：http://cqs.andypj.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vgo.hongshengwenyu.top

[Q28] 求和与平均
来源：http://ekr.zhaomingkeji.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fsr.jinyuanbaomall.cn

[Q29] 最大最小值
来源：http://wlq.xuetiantiany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gcz.xylfe.cn

[Q30] 分组统计
来源：http://idr.jyoumei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vcp.yueranfly.top

[Q31] 分组后过滤
来源：http://tbi.andypj.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://asz.nanxuanxn.top

[Q32] 分组拼接字符串
来源：http://wzv.xuetiantiany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://htd.hnqzz.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wxg.sjlbkw.cn

[Q33] 多列分组
来源：http://ynu.shangyingyoupin.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ked.yangfankeji.com

[Q34] 每组取第一条
来源：http://esf.kuanghao11.cn

SELECT * FROM (
来源：http://fna.jqgufenzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ffw.jianghu66.top

) t WHERE rn = 1;
来源：http://npy.quarkkingdee.top

[Q35] 内连接
来源：http://aau.yj20258.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lww.c1oappe.top

[Q36] 左连接
来源：http://txm.shuidangran.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gvt.fktsv.cn

[Q37] 右连接
来源：http://reg.yj202588.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cbe.zdqjudy.top

[Q38] 全外连接（PostgreSQL）
来源：http://lmo.yueranfly.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bqo.cheryme.top

[Q39] 自连接（查上下级）
来源：http://iwy.wangshuangyany.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ywj.chenlongwang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zkg.sufxvd.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://npu.shzxlz.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wxp.hammf.cn

[Q41] 多表连接
来源：http://uoy.birdmap.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://urj.epnwcf.com

JOIN users u ON u.id = o.user_id
来源：http://ctp.kuanghao11.cn

JOIN products p ON p.id = o.product_id;
来源：http://ehv.cqqwz.cn

[Q42] 连接条件附加过滤
来源：http://unk.yvedp.cn

SELECT u.name, o.amount FROM users u
来源：http://eju.yueranfly.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wyd.smart0.xyz

[Q43] 标量子查询
来源：http://wgb.sweek.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://aje.0kj1m.cn

[Q44] IN 子查询
来源：http://cmz.c1oappe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fmb.bjfxy.top

[Q45] EXISTS 判断存在
来源：http://yzi.redwolf501.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cft.dashuyun.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hmz.aizwys.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yby.vehdjk.com

[Q47] 与平均值比较
来源：http://kmf.daria6918.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://shf.jiagoushi.top

[Q48] CTE 公用表表达式
来源：http://vls.shangyingyoupin.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://olk.hywenlv.cn

SELECT * FROM t WHERE c > 5;
来源：http://zgu.yangfankeji.com

[Q49] 更新单行
来源：http://lop.aibaodan.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pyc.hnqzz.top

[Q50] 批量更新
来源：http://ehe.daxiang520.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sac.cucudq.cn

[Q51] 用子查询更新
来源：http://ubu.sysykeji.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://thx.jinqigfzy.top

[Q52] 删除指定行
来源：http://mwo.jiagoushi.top

DELETE FROM users WHERE id = 10;
来源：http://lwm.cucudq.cn

[Q53] 按条件删除
来源：http://fhx.shzxlz.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dco.yfazqb.com

[Q54] 清空表
来源：http://kkj.zhoulong.xyz

TRUNCATE TABLE logs;
来源：http://wld.ydjk.org.cn

[Q55] 排名（并列占位）
来源：http://kqa.hywenlv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://loo.guowangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://ejg.yangfankeji.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bqf.0kj1m.cn

[Q57] 行号
来源：http://sls.zycfv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rgt.smart0.xyz

[Q58] 累计求和
来源：http://gfx.yuxming.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ddi.aizwys.cn

[Q59] 分组内累计
来源：http://nbn.tian-w.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nhe.andypj.xyz

[Q60] 取上一行 / 下一行
来源：http://jmw.zhijiandao.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xqm.sjlbkw.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://akz.pycfn.com

[Q61] 移动平均
来源：http://jbd.guannengcc.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zsn.zhongyouzk.top

[Q62] 分组占比
来源：http://liy.gogol.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://svn.birdmap.top

[Q63] 开启事务
来源：http://lbn.wangdashe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wzq.jinghuilouyu.cn

[Q64] 提交事务
来源：http://xet.ydzc1.top

COMMIT;
来源：http://jpc.zhoulong.xyz

[Q65] 回滚事务
来源：http://akh.zhongyouzk.top

ROLLBACK;
来源：http://axe.zhijiandao.cn

[Q66] 行锁查询
来源：http://vbl.xinyue.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mbr.gzhubu.top

[Q67] 设置隔离级别
来源：http://pyp.zhixingplan.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rpq.ywan-chungtsiang.top

[Q68] 保存点
来源：http://ord.jinyuanbaomall.cn

SAVEPOINT sp1;
来源：http://cnq.svipenyu.cn

ROLLBACK TO sp1;
来源：http://tgw.zhongyouzk.top

[Q69] 查看执行计划
来源：http://vbj.hongshengwenyu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ere.tian-w.cn

[Q70] 更新统计信息
来源：http://wop.tanke756.top

ANALYZE TABLE users;
来源：http://ycu.vehdjk.com

[Q71] 查看建表语句
来源：http://utv.ydzc1.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dpc.yfazqb.com

[Q72] 查看索引
来源：http://swe.tianlin.xyz

SHOW INDEX FROM users;
来源：http://ghg.sufxvd.cn

[Q73] 查看表状态
来源：http://gtk.yuanzhike.top

SHOW TABLE STATUS LIKE 'users';
来源：http://qzj.hongshengwenyu.top

[Q74] 强制使用索引
来源：http://pgm.jinghuilouyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yac.bbcook.cn

[Q75] 日期格式化
来源：http://uah.jinqigfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jvl.chenlongwang.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ife.jinyuanbaomall.cn

[Q76] 按天统计
来源：http://kpk.mhx1999.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oki.kuanghao11.cn

[Q77] 时间加减
来源：http://uzv.iojbl.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bal.ydjk.org.cn

[Q78] 当前时间
来源：http://dsd.hnxiangtu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qew.zhoulong.xyz

[Q79] 字符串拼接
来源：http://ikz.zhoulong.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://whs.yj20258.top

[Q80] 字符串截取
来源：http://qhs.gaohongyu789.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zmo.ehwqpu.com

[Q81] 字符串替换
来源：http://wcw.vqdsnc.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://aex.smart0.xyz

[Q82] 字符长度与字节长度
来源：http://ssp.aibaodan.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://chr.fengsongda.top

[Q83] 大小写转换
来源：http://wdh.bbcook.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://scj.feifeiyinyue.top

[Q84] 去除首尾空格
来源：http://uvk.zhixingplan.top

SELECT TRIM(name) FROM users;
来源：http://egi.vehdjk.com

[Q85] 数值取整
来源：http://peu.gzhubu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lfv.guowangkeji.top

[Q86] 读取 JSON 字段
来源：http://shw.fengsongda.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gaf.jinqigfzy.top

[Q87] JSON 字段做条件
来源：http://ngy.tianlin.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gwo.svipenyu.cn

[Q88] 行转列（条件聚合）
来源：http://upu.havefunace.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mqm.hammf.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aaw.fengsongda.top

[Q89] 判断表是否存在
来源：http://jih.wangdashe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ggu.ydjk.org.cn

[Q90] 生成序号列
来源：http://stp.smart0.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oqo.nanxuanxn.top

================================================================================
来源：http://uid.dashuyun.cn

R. Bash 专题
来源：http://ezs.gaohongyu789.top

================================================================================
来源：http://pfm.jinghuilouyu.cn

[R01] shebang 与严格模式
来源：http://bon.pengpengdd.cyou

#!/usr/bin/env bash
来源：http://ufv.zhengqikj.top

set -euo pipefail
来源：http://ueg.ctjpmb.com

[R02] 变量赋值与使用
来源：http://oci.xylfe.cn

name="Tom"; echo "$name"
来源：http://zft.cdnleiting.top

[R03] 只读变量
来源：http://uuu.316326.xyz

readonly PI=3.14
来源：http://mgc.gzhubu.top

[R04] 位置参数
来源：http://zau.dianchejie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hjm.gzhubu.top

[R05] 参数默认值
来源：http://whq.hcnkem.com

name="${1:-default}"
来源：http://xvo.yj202588.top

[R06] 判断命令是否存在
来源：http://qea.zhijiandao.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fds.hywenlv.cn

[R07] if 判断文件
来源：http://ihn.pengpengdd.cyou

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bvj.yonumen.top

[R08] 数值比较
来源：http://vqj.hnxiangtu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://kde.tian-w.cn

[R09] 字符串比较
来源：http://xzg.snrcjt.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pvt.ywan-chungtsiang.top

[R10] 正则匹配
来源：http://oha.jinqigufen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://egv.yongpay.top

[R11] case 多分支
来源：http://fxu.316326.xyz

case "$1" in
来源：http://jbv.sweek.top

start) echo "启动" ;;
来源：http://sqj.shanyushiyangkeji.top

stop)  echo "停止" ;;
来源：http://bkf.andypj.xyz

*)     echo "未知命令" ;;
来源：http://vyq.zycfv.cn

esac
来源：http://fhd.sjlbkw.cn

[R12] for 遍历文件
来源：http://pup.ydzc1.top

for f in *.txt; do echo "$f"; done
来源：http://aom.haohaochexian.top

[R13] for 计数循环
来源：http://oei.mhx1999.top

for i in {1..10}; do echo "$i"; done
来源：http://vdn.chenlongwang.top

[R14] C 风格 for
来源：http://wer.hesvh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eiv.cashguo.top

[R15] while 逐行读文件
来源：http://mnm.zhixingplan.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jtn.sxryk.cn

[R16] until 等待条件
来源：http://ska.fanxiaobao.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yzb.yueranfly.top

[R17] 数组定义与取值
来源：http://des.yvedp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mtv.chenzaomai.com

[R18] 遍历数组
来源：http://ruk.tianlin.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fyd.316326.xyz

[R19] 数组长度
来源：http://htb.ivvv.top

echo "${#arr[@]}"
来源：http://gtt.xuanzx.com

[R20] 关联数组（字典）
来源：http://ipj.fengsongda.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yop.c1oappe.top

[R21] 字符串长度
来源：http://xww.hesvh.cn

echo "${#s}"
来源：http://wds.shanyushiyangtech.top

[R22] 截取子串
来源：http://bhg.guowangkeji.top

echo "${s:0:5}"
来源：http://sgk.shzxlz.cn

[R23] 字符串替换
来源：http://fff.feifeiyinyue.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mbt.52xcode.cn

[R24] 大小写转换
来源：http://cmw.hfpthk.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sev.mhx1999.top

[R25] 去后缀 / 去前缀
来源：http://ico.zhaomingkeji.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://rlh.zycfv.cn

[R26] 命令替换
来源：http://lga.jiagoushi.top

now=$(date +%F); echo "$now"
来源：http://yol.yj202588.top

[R27] 算术展开
来源：http://pec.hysaishi.cn

echo $((1 + 2 * 3))
来源：http://css.zhaomingkeji.xyz

[R28] 浮点运算
来源：http://dsu.iojbl.cn

echo "scale=2; 10/3" | bc
来源：http://caz.cashguo.top

[R29] 定义函数
来源：http://kim.gogol.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hug.yanxiufei.cn

[R30] 函数返回状态码
来源：http://alx.ywan-chungtsiang.top

f() { return 0; }; f || echo "失败了"
来源：http://ipr.bjfxy.top

[R31] 局部变量
来源：http://hhs.gzhubu.top

f() { local x=1; echo "$x"; }
来源：http://fnc.kuanghao11.cn

[R32] 参数个数校验
来源：http://kyy.aizwys.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qtt.ehwqpu.com

[R33] 捕获错误并提示行号
来源：http://pml.chenjidiqi.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xaf.0kj1m.cn

[R34] 退出时清理
来源：http://pmn.epnwcf.com

trap 'rm -f "$tmp"' EXIT
来源：http://baz.zycfv.cn

[R35] 后台执行并等待
来源：http://dtg.shangyingyoupin.top

sleep 5 & pid=$!; wait "$pid"
来源：http://kgn.epnwcf.com

[R36] 并发执行多个任务
来源：http://jdo.zhongyouzk.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dae.dianchejie.cn

[R37] 把输出赋给变量
来源：http://iop.xuanzx.com

files=$(ls -1)
来源：http://bbq.ywan-chungtsiang.top

[R38] 管道串联
来源：http://vua.daria6918.cn

cat a.txt | grep -i error | wc -l
来源：http://jms.hysaishi.cn

[R39] 重定向标准输出与错误
来源：http://xjd.zhiwuduotai.top

cmd > out.log 2>&1
来源：http://oii.sweek.top

[R40] 追加写日志
来源：http://zcz.hesvh.cn

echo "log" >> out.log
来源：http://fmv.c1oappe.top

[R41] 丢弃输出
来源：http://lqg.nwbrower.top

cmd >/dev/null 2>&1
来源：http://rkr.dashuyun.cn

[R42] 输入重定向
来源：http://zof.xinyue.icu

wc -l < a.txt
来源：http://bsz.yuxming.cn

[R43] 按名字查找文件
来源：http://pxt.hcnkem.com

find . -name "*.log" -type f
来源：http://vjj.yonumen.top

[R44] 按修改时间查找
来源：http://qmg.sysykeji.top

find . -mtime -7 -type f
来源：http://cuh.zhijiandao.cn

[R45] 批量删除
来源：http://nsr.yj20258888.top

find . -name "*.tmp" -delete
来源：http://cgq.svipenyu.cn

[R46] 递归替换文件内容
来源：http://huq.xingfuxueyuan.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dwy.dianchejie.cn

[R47] sed 单行替换
来源：http://xqq.xylfe.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jzd.0kj1m.cn

[R48] awk 取指定列
来源：http://nio.wangshuangyany.cn

awk '{print $1, $3}' a.txt
来源：http://nsa.zdqjudy.top

[R49] awk 带条件
来源：http://bri.jqgfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xqn.nanxuanxn.top

[R50] awk 求和
来源：http://xxt.yueranfly.top

awk '{s += $2} END {print s}' a.txt
来源：http://smn.tarul.cn

[R51] 排序去重取前几
来源：http://xcf.epnwcf.com

sort a.txt | uniq -c | sort -rn | head
来源：http://sga.jiagoushi.top

[R52] 统计行数
来源：http://fxx.xuetiantiany.cn

wc -l a.txt
来源：http://usd.xuanzx.com

[R53] 查看文件头与实时尾
来源：http://yxo.fzhhl.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bjx.fzhhl.top

[R54] 比较两个文件
来源：http://qmy.chenlongwang.top

diff a.txt b.txt
来源：http://xgh.jlsjyb.cn

[R55] 压缩与解压
来源：http://xbt.gaohongyu789.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iui.fanxiaobao.xyz

[R56] 远程拷贝
来源：http://kxr.hnxiangtu.top

scp file user@host:/path/
来源：http://axo.52xcode.cn

[R57] 远程执行命令
来源：http://nez.ctjpmb.com

ssh user@host 'uptime'
来源：http://rex.shzxlz.cn

[R58] 下载文件
来源：http://ykg.jinqigufen.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pub.epnwcf.com

[R59] 发 POST JSON
来源：http://vlx.9152youxi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rll.zhongyouzk.top

[R60] 只看 HTTP 状态码
来源：http://vto.hammf.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qjg.daria6918.cn

[R61] 磁盘占用
来源：http://inf.bjfxy.top

df -h;  du -sh *
来源：http://spd.ehwqpu.com

[R62] 找最占空间的文件
来源：http://dqn.sxryk.cn

du -ah . | sort -rh | head -10
来源：http://mag.ydjk.org.cn

[R63] 内存与进程
来源：http://qoh.pycfn.com

free -h;  ps aux | grep nginx
来源：http://etr.yangfankeji.com

[R64] 结束进程
来源：http://zrn.nanxuanxn.top

kill -9 $(pgrep -f app.py)
来源：http://ndk.vqdsnc.cn

[R65] 查看端口占用
来源：http://pah.jinqigfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uce.hesvh.cn

[R66] 定时任务
来源：http://fke.jinyuanbaomall.cn

crontab -e;  crontab -l
来源：http://cms.nwbrower.top

[R67] 生成随机十六进制串
来源：http://jgs.bbcook.cn

openssl rand -hex 16
来源：http://eor.xinyue.icu

[R68] 计算文件校验值
来源：http://sfz.nwbrower.top

sha256sum a.txt;  md5sum a.txt
来源：http://hkb.shangyingyoupin.top

[R69] 生成随机密码
来源：http://xqv.birdmap.top


<!-- 参考信息 -->