代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vif.vqdsnc.cn

[Q24] 去重
来源：http://aau.gzhubu.top

SELECT DISTINCT city FROM users;
来源：http://psu.xuetiantiany.cn

[Q25] 只取前 N 条
来源：http://btf.hammf.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nsl.kuanghao11.cn

[Q26] 计数
来源：http://vav.fehbvm.com

SELECT COUNT(*) FROM users;
来源：http://pqw.yfazqb.com

[Q27] 条件计数
来源：http://rke.yuanzhike.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xxr.cdnleiting.top

[Q28] 求和与平均
来源：http://gbc.vqdsnc.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://prq.cqqwz.cn

[Q29] 最大最小值
来源：http://rbk.jqgfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xsw.dashuyun.cn

[Q30] 分组统计
来源：http://dlx.smart0.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wje.nwbrower.top

[Q31] 分组后过滤
来源：http://fwn.pengpengdd.cyou

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uwu.sysykeji.top

[Q32] 分组拼接字符串
来源：http://vpm.xziqi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://joj.guowangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eqt.epnwcf.com

[Q33] 多列分组
来源：http://wao.ctjpmb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rkm.shanyushiyangkeji.top

[Q34] 每组取第一条
来源：http://drx.yj202588.top

SELECT * FROM (
来源：http://doz.shanyushiyangkeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://juy.316326.xyz

) t WHERE rn = 1;
来源：http://wjn.snrcjt.cn

[Q35] 内连接
来源：http://ayw.jinqigufen.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jhu.havefunace.top

[Q36] 左连接
来源：http://okw.zycfv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fss.hywenlv.cn

[Q37] 右连接
来源：http://ytt.iojbl.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hwi.ydzc1.top

[Q38] 全外连接（PostgreSQL）
来源：http://tlz.hnqzz.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://piu.cashguo.top

[Q39] 自连接（查上下级）
来源：http://oju.pengpengdd.cyou

SELECT e.name, m.name AS manager FROM employees e
来源：http://qea.jqgfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sdw.fanxiaobao.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://vec.vqdsnc.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kxp.bjfxy.top

[Q41] 多表连接
来源：http://ygy.kuanghao11.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://crk.kuanghao11.cn

JOIN users u ON u.id = o.user_id
来源：http://pmk.nwbrower.top

JOIN products p ON p.id = o.product_id;
来源：http://xfn.meibo888.top

[Q42] 连接条件附加过滤
来源：http://qni.ybcxt.top

SELECT u.name, o.amount FROM users u
来源：http://qlt.mhx1999.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xvi.haohaochexian.top

[Q43] 标量子查询
来源：http://mzs.ivvv.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dso.chenzaomai.com

[Q44] IN 子查询
来源：http://nwy.zhaomingkeji.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rmi.yj20258888.top

[Q45] EXISTS 判断存在
来源：http://dyi.hammf.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mlg.yj20258.top

[Q46] NOT EXISTS 判断不存在
来源：http://qgl.hywenlv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wjn.wangshuangyany.cn

[Q47] 与平均值比较
来源：http://oty.chenjidiqi.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://odf.shanyushiyangkeji.top

[Q48] CTE 公用表表达式
来源：http://fzj.chenzaomai.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wbo.52xcode.cn

SELECT * FROM t WHERE c > 5;
来源：http://ehq.xinyue.icu

[Q49] 更新单行
来源：http://oud.jianghu66.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qor.aibaodan.cn

[Q50] 批量更新
来源：http://ldi.hfpthk.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xfd.cheryme.top

[Q51] 用子查询更新
来源：http://gmg.ydjk.org.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://azo.ivvv.top

[Q52] 删除指定行
来源：http://pxh.hammf.cn

DELETE FROM users WHERE id = 10;
来源：http://ual.cdnleiting.top

[Q53] 按条件删除
来源：http://jdy.wangdashe.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://iat.daxiang520.top

[Q54] 清空表
来源：http://ump.316326.xyz

TRUNCATE TABLE logs;
来源：http://gnd.zhoulong.xyz

[Q55] 排名（并列占位）
来源：http://thw.zdbjq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wsi.fehbvm.com

[Q56] 密集排名（并列不占位）
来源：http://wkk.yuanzhike.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xyc.chenzaomai.com

[Q57] 行号
来源：http://igb.gogol.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wip.ybcxt.top

[Q58] 累计求和
来源：http://iwn.zhiwuduotai.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vlj.9152youxi.cn

[Q59] 分组内累计
来源：http://dvc.316326.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qyc.316326.xyz

[Q60] 取上一行 / 下一行
来源：http://bjn.gzhubu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uso.yueranfly.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://whn.quarkkingdee.top

[Q61] 移动平均
来源：http://jxm.ydjk.org.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uva.316326.xyz

[Q62] 分组占比
来源：http://anf.quarkkingdee.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dux.kuanghao11.cn

[Q63] 开启事务
来源：http://lsc.vqdsnc.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qjs.xingfuxueyuan.xyz

[Q64] 提交事务
来源：http://frm.yj20258888.top

COMMIT;
来源：http://jzi.aizwys.cn

[Q65] 回滚事务
来源：http://wpn.yj20258888.top

ROLLBACK;
来源：http://bra.cqqwz.cn

[Q66] 行锁查询
来源：http://mzz.yonumen.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qzy.vqdsnc.cn

[Q67] 设置隔离级别
来源：http://xsn.nanxuanxn.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dlr.jlsjyb.cn

[Q68] 保存点
来源：http://qac.vehdjk.com

SAVEPOINT sp1;
来源：http://kku.daria6918.cn

ROLLBACK TO sp1;
来源：http://kbl.jqgfzy.top

[Q69] 查看执行计划
来源：http://rpo.fzhhl.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cfj.quarkkingdee.top

[Q70] 更新统计信息
来源：http://pvl.quarkkingdee.top

ANALYZE TABLE users;
来源：http://xwg.jinqigufen.top

[Q71] 查看建表语句
来源：http://lfv.tianlin.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mof.ivvv.top

[Q72] 查看索引
来源：http://nxe.zhongyouzk.top

SHOW INDEX FROM users;
来源：http://zpy.shuidangran.top

[Q73] 查看表状态
来源：http://hyd.hfpthk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://paw.jinqigfzy.top

[Q74] 强制使用索引
来源：http://rif.feifeiyinyue.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nkv.andypj.xyz

[Q75] 日期格式化
来源：http://qpe.sweek.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://spt.chenzaomai.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://taq.xuanzx.com

[Q76] 按天统计
来源：http://bzp.sjlbkw.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://acr.xziqi.cn

[Q77] 时间加减
来源：http://edt.yangfankeji.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mto.quarkkingdee.top

[Q78] 当前时间
来源：http://hnv.sxryk.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ecd.jinqigfzy.top

[Q79] 字符串拼接
来源：http://ift.bbcook.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sfj.jinqigufen.top

[Q80] 字符串截取
来源：http://xdi.sxryk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vrv.hammf.cn

[Q81] 字符串替换
来源：http://cew.haohaochexian.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://czk.jlsjyb.cn

[Q82] 字符长度与字节长度
来源：http://jgw.vqdsnc.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jwl.ivvv.top

[Q83] 大小写转换
来源：http://muv.sufxvd.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ban.ivvv.top

[Q84] 去除首尾空格
来源：http://gdo.zdqjudy.top

SELECT TRIM(name) FROM users;
来源：http://owg.vqdsnc.cn

[Q85] 数值取整
来源：http://cnh.hesvh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fss.xuanzx.com

[Q86] 读取 JSON 字段
来源：http://qbx.c1oappe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fax.hnqzz.top

[Q87] JSON 字段做条件
来源：http://uim.tarul.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gvs.hammf.cn

[Q88] 行转列（条件聚合）
来源：http://djx.epnwcf.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mlo.yvedp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xlb.jiagoushi.top

[Q89] 判断表是否存在
来源：http://nzq.nanxinkj.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dxo.smart0.xyz

[Q90] 生成序号列
来源：http://luc.shzxlz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://osq.andypj.xyz

================================================================================
来源：http://put.pengpengdd.cyou

R. Bash 专题
来源：http://iof.jinghuilouyu.cn

================================================================================
来源：http://dhd.nanxinkj.top

[R01] shebang 与严格模式
来源：http://mhg.jiagoushi.top

#!/usr/bin/env bash
来源：http://ymo.ywan-chungtsiang.top

set -euo pipefail
来源：http://ngm.zhixingplan.top

[R02] 变量赋值与使用
来源：http://vit.hysaishi.cn

name="Tom"; echo "$name"
来源：http://vcw.dashuyun.cn

[R03] 只读变量
来源：http://iok.cucudq.cn

readonly PI=3.14
来源：http://zwk.birdmap.top

[R04] 位置参数
来源：http://vxx.zhixingplan.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jhl.uphjek.com

[R05] 参数默认值
来源：http://llq.feifeiyinyue.top

name="${1:-default}"
来源：http://fep.kuanghao11.cn

[R06] 判断命令是否存在
来源：http://exc.andypj.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nef.9152youxi.cn

[R07] if 判断文件
来源：http://cks.ppjwa.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ktm.jyoumei.cn

[R08] 数值比较
来源：http://odc.ywan-chungtsiang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ksx.daxiang520.top

[R09] 字符串比较
来源：http://vzi.jinyuanbaomall.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xtc.ywan-chungtsiang.top

[R10] 正则匹配
来源：http://yhw.hongshengwenyu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rew.jyoumei.cn

[R11] case 多分支
来源：http://kiw.fzhhl.top

case "$1" in
来源：http://edx.xylfe.cn

start) echo "启动" ;;
来源：http://yvi.cdnleiting.top

stop)  echo "停止" ;;
来源：http://nwi.chenlongwang.top

*)     echo "未知命令" ;;
来源：http://mee.tianlin.xyz

esac
来源：http://ifu.tanke756.top

[R12] for 遍历文件
来源：http://kwr.andypj.xyz

for f in *.txt; do echo "$f"; done
来源：http://cxw.redwolf501.top

[R13] for 计数循环
来源：http://mzw.fanxiaobao.xyz

for i in {1..10}; do echo "$i"; done
来源：http://vhy.feifeiyinyue.top

[R14] C 风格 for
来源：http://nmh.jinqigufen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zew.bjfxy.top

[R15] while 逐行读文件
来源：http://zrf.zhoulong.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bla.daxiang520.top

[R16] until 等待条件
来源：http://nbw.yangfankeji.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dmc.wangshuangyany.cn

[R17] 数组定义与取值
来源：http://byu.snrcjt.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sgm.zdqjudy.top

[R18] 遍历数组
来源：http://zcu.chenzaomai.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ppm.ppjwa.cn

[R19] 数组长度
来源：http://ubf.sjlbkw.cn

echo "${#arr[@]}"
来源：http://mbs.xuanzx.com

[R20] 关联数组（字典）
来源：http://mya.redwolf501.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zaa.bjfxy.top

[R21] 字符串长度
来源：http://nzr.andypj.xyz

echo "${#s}"
来源：http://ejw.ehwqpu.com

[R22] 截取子串
来源：http://dan.andypj.xyz

echo "${s:0:5}"
来源：http://otw.dianchejie.cn

[R23] 字符串替换
来源：http://hwr.vqdsnc.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xqe.ctjpmb.com

[R24] 大小写转换
来源：http://aof.fengsongda.top

echo "${s^^}"; echo "${s,,}"
来源：http://cpe.zhijiandao.cn

[R25] 去后缀 / 去前缀
来源：http://eip.gaohongyu789.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://cpi.guannengcc.top

[R26] 命令替换
来源：http://ycb.quarkkingdee.top

now=$(date +%F); echo "$now"
来源：http://jyq.tarul.cn

[R27] 算术展开
来源：http://hhp.redwolf501.top

echo $((1 + 2 * 3))
来源：http://icc.sjlbkw.cn

[R28] 浮点运算
来源：http://rid.vqdsnc.cn

echo "scale=2; 10/3" | bc
来源：http://rzg.fktsv.cn

[R29] 定义函数
来源：http://dll.zhoulong.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kfu.jiagoushi.top

[R30] 函数返回状态码
来源：http://fcx.aibaodan.cn

f() { return 0; }; f || echo "失败了"
来源：http://eff.tian-w.cn

[R31] 局部变量
来源：http://hyt.hywenlv.cn

f() { local x=1; echo "$x"; }
来源：http://ivt.bjfxy.top

[R32] 参数个数校验
来源：http://nfs.yonumen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ldy.hysaishi.cn

[R33] 捕获错误并提示行号
来源：http://ive.bjfxy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zrq.xylfe.cn

[R34] 退出时清理
来源：http://qix.hesvh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://drp.havefunace.top

[R35] 后台执行并等待
来源：http://kcb.bjfxy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://pbz.xuetiantiany.cn

[R36] 并发执行多个任务
来源：http://smn.yfazqb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fym.jqgfzy.top

[R37] 把输出赋给变量
来源：http://boh.dashuyun.cn

files=$(ls -1)
来源：http://nbt.shzxlz.cn

[R38] 管道串联
来源：http://agk.daria6918.cn

cat a.txt | grep -i error | wc -l
来源：http://xau.pengpengdd.cyou

[R39] 重定向标准输出与错误
来源：http://del.zhixingplan.top

cmd > out.log 2>&1
来源：http://zpa.xingfuxueyuan.xyz

[R40] 追加写日志
来源：http://euf.yj20258888.top

echo "log" >> out.log
来源：http://sbw.birdmap.top

[R41] 丢弃输出
来源：http://ccw.fktsv.cn

cmd >/dev/null 2>&1
来源：http://vha.ybcxt.top

[R42] 输入重定向
来源：http://han.gaohongyu789.top

wc -l < a.txt
来源：http://ozk.tianlin.xyz

[R43] 按名字查找文件
来源：http://lrf.yuxming.cn

find . -name "*.log" -type f
来源：http://fit.jyoumei.cn

[R44] 按修改时间查找
来源：http://vzc.shangyingyoupin.top

find . -mtime -7 -type f
来源：http://wyf.zhongyouzk.top

[R45] 批量删除
来源：http://izt.shuidangran.top

find . -name "*.tmp" -delete
来源：http://gsf.hammf.cn

[R46] 递归替换文件内容
来源：http://kpu.chenzaomai.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zvy.yongpay.top

[R47] sed 单行替换
来源：http://rzt.dianchejie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xwt.nwbrower.top

[R48] awk 取指定列
来源：http://vtl.yueranfly.top

awk '{print $1, $3}' a.txt
来源：http://xqq.yj20258.top

[R49] awk 带条件
来源：http://kua.cqqwz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ckp.haohaochexian.top

[R50] awk 求和
来源：http://vzc.zhongyouzk.top

awk '{s += $2} END {print s}' a.txt
来源：http://kbt.jianghu66.top

[R51] 排序去重取前几
来源：http://him.ppjwa.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mez.jiagoushi.top

[R52] 统计行数
来源：http://zhy.ydjk.org.cn

wc -l a.txt
来源：http://qxs.hcnkem.com

[R53] 查看文件头与实时尾
来源：http://fnh.gotoacloud.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ywy.sjlbkw.cn

[R54] 比较两个文件
来源：http://hns.dianchejie.cn

diff a.txt b.txt
来源：http://wll.pycfn.com

[R55] 压缩与解压
来源：http://aid.quarkkingdee.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://phg.jiagoushi.top

[R56] 远程拷贝
来源：http://dpg.chenjidiqi.icu

scp file user@host:/path/
来源：http://nlm.kuanghao11.cn

[R57] 远程执行命令
来源：http://lpo.fanxiaobao.xyz

ssh user@host 'uptime'
来源：http://qri.chenjidiqi.icu

[R58] 下载文件
来源：http://icp.shzxlz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mej.dashuyun.cn

[R59] 发 POST JSON
来源：http://rfe.pycfn.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fod.zdqjudy.top

[R60] 只看 HTTP 状态码
来源：http://iqe.sufxvd.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zpt.316326.xyz

[R61] 磁盘占用
来源：http://rza.zycfv.cn

df -h;  du -sh *
来源：http://xfx.yueranfly.top

[R62] 找最占空间的文件
来源：http://lbh.nanxuanxn.top

du -ah . | sort -rh | head -10
来源：http://qel.cashguo.top

[R63] 内存与进程
来源：http://nge.jinghuilouyu.cn

free -h;  ps aux | grep nginx
来源：http://axi.hesvh.cn

[R64] 结束进程
来源：http://yaf.ivvv.top

kill -9 $(pgrep -f app.py)
来源：http://nnu.dashuyun.cn

[R65] 查看端口占用
来源：http://dtm.52xcode.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jaz.zhixingplan.top

[R66] 定时任务
来源：http://gfx.yanxiufei.cn

crontab -e;  crontab -l
来源：http://ueo.xylfe.cn

[R67] 生成随机十六进制串
来源：http://gdm.daria6918.cn

openssl rand -hex 16
来源：http://nlp.9152youxi.cn

[R68] 计算文件校验值
来源：http://ogk.zdbjq.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kzz.epnwcf.com

[R69] 生成随机密码
来源：http://ujx.wangdashe.top

head -c 16 /dev/urandom | base64
来源：http://krw.jinyuanbaomall.cn

[R70] 时间戳与互转
来源：http://mno.cucudq.cn

date +%s;  date -d @1700000000
来源：http://ffk.yanxiufei.cn

[R71] 日期格式化
来源：http://tvp.yonumen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nym.meibo888.top

[R72] 等待端口就绪
来源：http://ruz.shanyushiyangtech.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nwj.nanxuanxn.top

[R73] 分割大日志
来源：http://jui.bjfxy.top


<!-- 参考信息 -->