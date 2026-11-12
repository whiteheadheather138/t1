代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sfj.hesvh.cn

[Q24] 去重
来源：http://kid.gaohongyu789.top

SELECT DISTINCT city FROM users;
来源：http://ubz.cqqwz.cn

[Q25] 只取前 N 条
来源：http://rym.ivvv.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zrc.yanxiufei.cn

[Q26] 计数
来源：http://qxc.pengpengdd.cyou

SELECT COUNT(*) FROM users;
来源：http://lgv.zhiwuduotai.top

[Q27] 条件计数
来源：http://xge.hfpthk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dwb.fanxiaobao.xyz

[Q28] 求和与平均
来源：http://vtb.yangfankeji.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xjd.yongpay.top

[Q29] 最大最小值
来源：http://qiz.xziqi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yyu.tarul.cn

[Q30] 分组统计
来源：http://fgr.fktsv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kwm.fehbvm.com

[Q31] 分组后过滤
来源：http://nrw.zhiwuduotai.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yby.hysaishi.cn

[Q32] 分组拼接字符串
来源：http://abg.zhixingplan.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ifw.tian-w.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dbn.zdqjudy.top

[Q33] 多列分组
来源：http://plj.zdqjudy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bij.yongpay.top

[Q34] 每组取第一条
来源：http://grd.zhongyouzk.top

SELECT * FROM (
来源：http://dbn.yj202588.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wrq.bbcook.cn

) t WHERE rn = 1;
来源：http://jza.yj202588.top

[Q35] 内连接
来源：http://unv.jyoumei.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wez.ywan-chungtsiang.top

[Q36] 左连接
来源：http://trp.epnwcf.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hyc.cdnleiting.top

[Q37] 右连接
来源：http://qvh.zhongyouzk.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://irq.yanxiufei.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wpx.fehbvm.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://eao.nanxinkj.top

[Q39] 自连接（查上下级）
来源：http://vzs.cqqwz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nvh.zhongyouzk.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yhu.yuxming.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://exj.fehbvm.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ohl.hongshengwenyu.top

[Q41] 多表连接
来源：http://fun.cheryme.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bev.yj20258.top

JOIN users u ON u.id = o.user_id
来源：http://wkc.smart0.xyz

JOIN products p ON p.id = o.product_id;
来源：http://igs.sxryk.cn

[Q42] 连接条件附加过滤
来源：http://lrn.shangyingyoupin.top

SELECT u.name, o.amount FROM users u
来源：http://mdg.chenlongwang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zpx.yonumen.top

[Q43] 标量子查询
来源：http://ibp.nanxuanxn.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ogl.yangfankeji.com

[Q44] IN 子查询
来源：http://tig.vqdsnc.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ckh.pycfn.com

[Q45] EXISTS 判断存在
来源：http://val.52xcode.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bba.pycfn.com

[Q46] NOT EXISTS 判断不存在
来源：http://tva.aizwys.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kfb.jqgufenzy.top

[Q47] 与平均值比较
来源：http://omj.sxryk.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cle.ywan-chungtsiang.top

[Q48] CTE 公用表表达式
来源：http://wlf.meibo888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fnu.zhaomingkeji.xyz

SELECT * FROM t WHERE c > 5;
来源：http://iid.jinqigfzy.top

[Q49] 更新单行
来源：http://ssi.gotoacloud.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kzn.yanxiufei.cn

[Q50] 批量更新
来源：http://rna.quarkkingdee.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ekw.hysaishi.cn

[Q51] 用子查询更新
来源：http://snb.yfazqb.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sxz.guowangkeji.top

[Q52] 删除指定行
来源：http://pkd.iojbl.cn

DELETE FROM users WHERE id = 10;
来源：http://qwf.chenlongwang.top

[Q53] 按条件删除
来源：http://wtk.fanxiaobao.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://crk.chenlongwang.top

[Q54] 清空表
来源：http://jtj.iojbl.cn

TRUNCATE TABLE logs;
来源：http://lvf.jyoumei.cn

[Q55] 排名（并列占位）
来源：http://ark.shuidangran.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fkw.guowangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://xnd.jqgufenzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://omg.pycfn.com

[Q57] 行号
来源：http://dxp.hcnkem.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://puc.guannengcc.top

[Q58] 累计求和
来源：http://fbs.jinqigfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kpo.zdqjudy.top

[Q59] 分组内累计
来源：http://wmn.sjlbkw.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xhw.yj202588.top

[Q60] 取上一行 / 下一行
来源：http://ecw.yongpay.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yvb.wangshuangyany.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qlz.bbcook.cn

[Q61] 移动平均
来源：http://wfw.yonumen.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cbf.yongpay.top

[Q62] 分组占比
来源：http://tir.yj20258888.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lqi.cucudq.cn

[Q63] 开启事务
来源：http://aly.316326.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://qmz.yj20258.top

[Q64] 提交事务
来源：http://igl.ydjk.org.cn

COMMIT;
来源：http://khl.haohaochexian.top

[Q65] 回滚事务
来源：http://cfg.ydzc1.top

ROLLBACK;
来源：http://qrr.ybcxt.top

[Q66] 行锁查询
来源：http://lcm.dashuyun.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iwx.hywenlv.cn

[Q67] 设置隔离级别
来源：http://lko.vehdjk.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yzk.ydjk.org.cn

[Q68] 保存点
来源：http://ljs.mhx1999.top

SAVEPOINT sp1;
来源：http://ftg.zhaomingkeji.xyz

ROLLBACK TO sp1;
来源：http://pos.xylfe.cn

[Q69] 查看执行计划
来源：http://zpe.jlsjyb.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://meq.epnwcf.com

[Q70] 更新统计信息
来源：http://nzj.hnqzz.top

ANALYZE TABLE users;
来源：http://qeo.chenjidiqi.icu

[Q71] 查看建表语句
来源：http://olq.jiagoushi.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fid.jinqigfzy.top

[Q72] 查看索引
来源：http://bzf.chenzaomai.com

SHOW INDEX FROM users;
来源：http://pja.cdnleiting.top

[Q73] 查看表状态
来源：http://mhw.quarkkingdee.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ddy.zycfv.cn

[Q74] 强制使用索引
来源：http://uxz.shanyushiyangtech.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://exa.jinghuilouyu.cn

[Q75] 日期格式化
来源：http://nyx.0kj1m.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ash.ppjwa.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qsh.haohaochexian.top

[Q76] 按天统计
来源：http://lgh.xinyue.icu

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uuv.sxryk.cn

[Q77] 时间加减
来源：http://sas.jinqigfzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://odp.redwolf501.top

[Q78] 当前时间
来源：http://glk.fengsongda.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nyv.tian-w.cn

[Q79] 字符串拼接
来源：http://fzu.vqdsnc.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qya.fanxiaobao.xyz

[Q80] 字符串截取
来源：http://vgf.smart0.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ozb.dianchejie.cn

[Q81] 字符串替换
来源：http://vxz.yueranfly.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://inl.jinqigfzy.top

[Q82] 字符长度与字节长度
来源：http://xdz.aibaodan.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blq.xuetiantiany.cn

[Q83] 大小写转换
来源：http://bom.guannengcc.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://das.iojbl.cn

[Q84] 去除首尾空格
来源：http://hgl.vehdjk.com

SELECT TRIM(name) FROM users;
来源：http://cmy.uphjek.com

[Q85] 数值取整
来源：http://ipg.havefunace.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://oog.tianlin.xyz

[Q86] 读取 JSON 字段
来源：http://bby.daxiang520.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vvs.aibaodan.cn

[Q87] JSON 字段做条件
来源：http://ylj.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rrg.tarul.cn

[Q88] 行转列（条件聚合）
来源：http://nbi.shzxlz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vbv.quarkkingdee.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eus.gaohongyu789.top

[Q89] 判断表是否存在
来源：http://vla.hongshengwenyu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lgy.0kj1m.cn

[Q90] 生成序号列
来源：http://dpa.kuanghao11.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pyf.jyoumei.cn

================================================================================
来源：http://ziy.shanyushiyangtech.top

R. Bash 专题
来源：http://maf.hammf.cn

================================================================================
来源：http://isr.cashguo.top

[R01] shebang 与严格模式
来源：http://sxf.52xcode.cn

#!/usr/bin/env bash
来源：http://fwe.aibaodan.cn

set -euo pipefail
来源：http://xys.andypj.xyz

[R02] 变量赋值与使用
来源：http://wcp.hywenlv.cn

name="Tom"; echo "$name"
来源：http://qkp.gotoacloud.top

[R03] 只读变量
来源：http://qyh.snrcjt.cn

readonly PI=3.14
来源：http://bky.yj20258.top

[R04] 位置参数
来源：http://gcw.c1oappe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iun.redwolf501.top

[R05] 参数默认值
来源：http://yul.ehwqpu.com

name="${1:-default}"
来源：http://gxy.cdnleiting.top

[R06] 判断命令是否存在
来源：http://pzz.yonumen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mdh.yj20258888.top

[R07] if 判断文件
来源：http://zpo.hnqzz.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lsm.hesvh.cn

[R08] 数值比较
来源：http://rvm.xziqi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ojv.hcnkem.com

[R09] 字符串比较
来源：http://nnd.nanxinkj.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fus.zhixingplan.top

[R10] 正则匹配
来源：http://fls.hysaishi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uqq.bjfxy.top

[R11] case 多分支
来源：http://bvp.havefunace.top

case "$1" in
来源：http://sdz.cheryme.top

start) echo "启动" ;;
来源：http://snc.yonumen.top

stop)  echo "停止" ;;
来源：http://yin.zdbjq.cn

*)     echo "未知命令" ;;
来源：http://ajx.cqqwz.cn

esac
来源：http://xbg.yongpay.top

[R12] for 遍历文件
来源：http://vdl.vqdsnc.cn

for f in *.txt; do echo "$f"; done
来源：http://rjv.yuxming.cn

[R13] for 计数循环
来源：http://usn.daria6918.cn

for i in {1..10}; do echo "$i"; done
来源：http://cqm.52xcode.cn

[R14] C 风格 for
来源：http://jur.c1oappe.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zaz.zhengqikj.top

[R15] while 逐行读文件
来源：http://tga.ehwqpu.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zwa.tianlin.xyz

[R16] until 等待条件
来源：http://osa.dashuyun.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hwl.fanxiaobao.xyz

[R17] 数组定义与取值
来源：http://qlq.sxryk.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ugr.ydzc1.top

[R18] 遍历数组
来源：http://iuk.jinqigfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://aly.xziqi.cn

[R19] 数组长度
来源：http://uum.nwbrower.top

echo "${#arr[@]}"
来源：http://tsc.aibaodan.cn

[R20] 关联数组（字典）
来源：http://fix.xziqi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tag.hnqzz.top

[R21] 字符串长度
来源：http://cpn.shangyingyoupin.top

echo "${#s}"
来源：http://rsr.xinyue.icu

[R22] 截取子串
来源：http://ttx.yuanzhike.top

echo "${s:0:5}"
来源：http://bew.ivvv.top

[R23] 字符串替换
来源：http://yyn.dianchejie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pjm.shanyushiyangkeji.top

[R24] 大小写转换
来源：http://tlq.zdqjudy.top

echo "${s^^}"; echo "${s,,}"
来源：http://ncr.vqdsnc.cn

[R25] 去后缀 / 去前缀
来源：http://vpg.jiagoushi.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mbw.ywan-chungtsiang.top

[R26] 命令替换
来源：http://vna.hysaishi.cn

now=$(date +%F); echo "$now"
来源：http://loi.aibaodan.cn

[R27] 算术展开
来源：http://btv.cashguo.top

echo $((1 + 2 * 3))
来源：http://vlh.zycfv.cn

[R28] 浮点运算
来源：http://qga.ehwqpu.com

echo "scale=2; 10/3" | bc
来源：http://dqc.jinyuanbaomall.cn

[R29] 定义函数
来源：http://zcp.redwolf501.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tur.xuanzx.com

[R30] 函数返回状态码
来源：http://ypn.wangshuangyany.cn

f() { return 0; }; f || echo "失败了"
来源：http://dgn.chenzaomai.com

[R31] 局部变量
来源：http://hha.quarkkingdee.top

f() { local x=1; echo "$x"; }
来源：http://hen.hongshengwenyu.top

[R32] 参数个数校验
来源：http://wvi.fehbvm.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gjx.pycfn.com

[R33] 捕获错误并提示行号
来源：http://ajk.gotoacloud.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rkm.jlsjyb.cn

[R34] 退出时清理
来源：http://kua.hnxiangtu.top

trap 'rm -f "$tmp"' EXIT
来源：http://ybn.jqgufenzy.top

[R35] 后台执行并等待
来源：http://omf.yj20258.top

sleep 5 & pid=$!; wait "$pid"
来源：http://eee.mhx1999.top

[R36] 并发执行多个任务
来源：http://eql.yuxming.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://udk.sufxvd.cn

[R37] 把输出赋给变量
来源：http://pyo.dashuyun.cn

files=$(ls -1)
来源：http://mmn.chenlongwang.top

[R38] 管道串联
来源：http://qjc.yj20258888.top

cat a.txt | grep -i error | wc -l
来源：http://usu.dashuyun.cn

[R39] 重定向标准输出与错误
来源：http://hag.yj20258888.top

cmd > out.log 2>&1
来源：http://zuu.meibo888.top

[R40] 追加写日志
来源：http://phi.cucudq.cn

echo "log" >> out.log
来源：http://lwe.xinyue.icu

[R41] 丢弃输出
来源：http://xuw.52xcode.cn

cmd >/dev/null 2>&1
来源：http://vpl.gogol.net.cn

[R42] 输入重定向
来源：http://ohi.pycfn.com

wc -l < a.txt
来源：http://jxm.tanke756.top

[R43] 按名字查找文件
来源：http://cqy.wangshuangyany.cn

find . -name "*.log" -type f
来源：http://rhn.bjfxy.top

[R44] 按修改时间查找
来源：http://xtc.vehdjk.com

find . -mtime -7 -type f
来源：http://wjd.nanxinkj.top

[R45] 批量删除
来源：http://rbz.pycfn.com

find . -name "*.tmp" -delete
来源：http://zwv.shanyushiyangkeji.top

[R46] 递归替换文件内容
来源：http://rbj.cheryme.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hne.jyoumei.cn

[R47] sed 单行替换
来源：http://apr.jinyuanbaomall.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yyj.xinyue.icu

[R48] awk 取指定列
来源：http://ovv.hfpthk.cn

awk '{print $1, $3}' a.txt
来源：http://gqt.birdmap.top

[R49] awk 带条件
来源：http://woj.zhaomingkeji.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nqo.haohaochexian.top

[R50] awk 求和
来源：http://inc.wangshuangyany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://teb.haohaochexian.top

[R51] 排序去重取前几
来源：http://bak.bbcook.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zgf.hfpthk.cn

[R52] 统计行数
来源：http://cms.daria6918.cn

wc -l a.txt
来源：http://qnk.hongshengwenyu.top

[R53] 查看文件头与实时尾
来源：http://qrc.zycfv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nvr.ehwqpu.com

[R54] 比较两个文件
来源：http://grw.ywan-chungtsiang.top

diff a.txt b.txt
来源：http://wrd.cashguo.top

[R55] 压缩与解压
来源：http://ckj.zhixingplan.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://irv.xingfuxueyuan.xyz

[R56] 远程拷贝
来源：http://mlx.vqdsnc.cn

scp file user@host:/path/
来源：http://doc.aizwys.cn

[R57] 远程执行命令
来源：http://jmg.epnwcf.com

ssh user@host 'uptime'
来源：http://qdn.chenzaomai.com

[R58] 下载文件
来源：http://nlu.xuetiantiany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ryz.ybcxt.top

[R59] 发 POST JSON
来源：http://lvd.jqgfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hxg.zhongyouzk.top

[R60] 只看 HTTP 状态码
来源：http://kfd.jiagoushi.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yyq.hysaishi.cn

[R61] 磁盘占用
来源：http://dof.epnwcf.com

df -h;  du -sh *
来源：http://rpg.cheryme.top

[R62] 找最占空间的文件
来源：http://hsj.jyoumei.cn

du -ah . | sort -rh | head -10
来源：http://gft.pycfn.com

[R63] 内存与进程
来源：http://aeh.shangyingyoupin.top

free -h;  ps aux | grep nginx
来源：http://kiw.shangyingyoupin.top

[R64] 结束进程
来源：http://dtv.zdbjq.cn

kill -9 $(pgrep -f app.py)
来源：http://rzt.guannengcc.top

[R65] 查看端口占用
来源：http://doi.ydjk.org.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lqg.zhixingplan.top

[R66] 定时任务
来源：http://ngz.sxryk.cn

crontab -e;  crontab -l
来源：http://zov.sxryk.cn

[R67] 生成随机十六进制串
来源：http://eny.zycfv.cn

openssl rand -hex 16
来源：http://hwr.xingfuxueyuan.xyz

[R68] 计算文件校验值
来源：http://hac.tarul.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jye.epnwcf.com

[R69] 生成随机密码
来源：http://gpm.iojbl.cn

head -c 16 /dev/urandom | base64
来源：http://klj.xylfe.cn

[R70] 时间戳与互转
来源：http://chw.hnqzz.top

date +%s;  date -d @1700000000
来源：http://mot.iojbl.cn

[R71] 日期格式化
来源：http://mvj.jinyuanbaomall.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xvv.jqgufenzy.top

[R72] 等待端口就绪
来源：http://wdi.jinyuanbaomall.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://see.jinyuanbaomall.cn

[R73] 分割大日志
来源：http://bou.nwbrower.top


<!-- 参考信息 -->