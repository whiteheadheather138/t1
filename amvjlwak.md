代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://ikv.snrcjt.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yys.epnwcf.com

[Q39] 自连接（查上下级）
来源：http://tbu.fanxiaobao.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://zks.tian-w.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yom.feifeiyinyue.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zyq.zhoulong.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cjv.0kj1m.cn

[Q41] 多表连接
来源：http://chw.hammf.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cmq.gaohongyu789.top

JOIN users u ON u.id = o.user_id
来源：http://rdk.meibo888.top

JOIN products p ON p.id = o.product_id;
来源：http://egn.gogol.net.cn

[Q42] 连接条件附加过滤
来源：http://axh.xinyue.icu

SELECT u.name, o.amount FROM users u
来源：http://ykp.svipenyu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pjw.chenjidiqi.icu

[Q43] 标量子查询
来源：http://aoq.ydjk.org.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fmo.sjlbkw.cn

[Q44] IN 子查询
来源：http://jvu.fehbvm.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jld.chenzaomai.com

[Q45] EXISTS 判断存在
来源：http://wcb.daria6918.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://otl.52xcode.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yyn.zdbjq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xve.zhengqikj.top

[Q47] 与平均值比较
来源：http://ogh.guowangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kek.shangyingyoupin.top

[Q48] CTE 公用表表达式
来源：http://uah.yangfankeji.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xzr.ppjwa.cn

SELECT * FROM t WHERE c > 5;
来源：http://wvl.zdqjudy.top

[Q49] 更新单行
来源：http://xhk.meibo888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wxh.xinyue.icu

[Q50] 批量更新
来源：http://toe.yj202588.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ncd.sweek.top

[Q51] 用子查询更新
来源：http://len.ivvv.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://les.fengsongda.top

[Q52] 删除指定行
来源：http://mfb.jinghuilouyu.cn

DELETE FROM users WHERE id = 10;
来源：http://wag.jinqigufen.top

[Q53] 按条件删除
来源：http://rix.jiagoushi.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xdg.xuetiantiany.cn

[Q54] 清空表
来源：http://uqa.xinyue.icu

TRUNCATE TABLE logs;
来源：http://osy.shanyushiyangkeji.top

[Q55] 排名（并列占位）
来源：http://ttm.xuetiantiany.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sxy.yj20258888.top

[Q56] 密集排名（并列不占位）
来源：http://ywr.bbcook.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hpt.shuidangran.top

[Q57] 行号
来源：http://vgl.snrcjt.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hju.svipenyu.cn

[Q58] 累计求和
来源：http://tna.meibo888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pnh.hammf.cn

[Q59] 分组内累计
来源：http://dwf.zhongyouzk.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cbd.jinqigufen.top

[Q60] 取上一行 / 下一行
来源：http://tbu.dianchejie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oke.fanxiaobao.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://csw.gogol.net.cn

[Q61] 移动平均
来源：http://hwx.tanke756.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cru.cdnleiting.top

[Q62] 分组占比
来源：http://dlm.jinqigufen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mlz.daxiang520.top

[Q63] 开启事务
来源：http://xlj.hywenlv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://top.hnxiangtu.top

[Q64] 提交事务
来源：http://brx.sysykeji.top

COMMIT;
来源：http://wwc.fanxiaobao.xyz

[Q65] 回滚事务
来源：http://snb.vehdjk.com

ROLLBACK;
来源：http://dmc.gogol.net.cn

[Q66] 行锁查询
来源：http://nzh.ivvv.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://okh.jqgfzy.top

[Q67] 设置隔离级别
来源：http://zxu.jianghu66.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hjh.9152youxi.cn

[Q68] 保存点
来源：http://ucc.birdmap.top

SAVEPOINT sp1;
来源：http://yxi.guowangkeji.top

ROLLBACK TO sp1;
来源：http://bpw.daria6918.cn

[Q69] 查看执行计划
来源：http://hwj.daria6918.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lim.chenzaomai.com

[Q70] 更新统计信息
来源：http://tvw.shanyushiyangtech.top

ANALYZE TABLE users;
来源：http://nlm.zhixingplan.top

[Q71] 查看建表语句
来源：http://idg.jinqigufen.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pvt.ybcxt.top

[Q72] 查看索引
来源：http://srr.jianghu66.top

SHOW INDEX FROM users;
来源：http://mza.xziqi.cn

[Q73] 查看表状态
来源：http://xtv.feifeiyinyue.top

SHOW TABLE STATUS LIKE 'users';
来源：http://fqn.wangshuangyany.cn

[Q74] 强制使用索引
来源：http://ryi.chenlongwang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hgo.hcnkem.com

[Q75] 日期格式化
来源：http://yxt.yj202588.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uoo.pycfn.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bfe.dashuyun.cn

[Q76] 按天统计
来源：http://whs.jinqigfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nex.sxryk.cn

[Q77] 时间加减
来源：http://tqk.aibaodan.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ory.dianchejie.cn

[Q78] 当前时间
来源：http://puk.iojbl.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://amv.yueranfly.top

[Q79] 字符串拼接
来源：http://ent.cucudq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xhw.fktsv.cn

[Q80] 字符串截取
来源：http://aoc.0kj1m.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rxs.fengsongda.top

[Q81] 字符串替换
来源：http://kgv.haohaochexian.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://myw.zhiwuduotai.top

[Q82] 字符长度与字节长度
来源：http://loy.cheryme.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nlz.zhoulong.xyz

[Q83] 大小写转换
来源：http://jdr.yangfankeji.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gqc.vqdsnc.cn

[Q84] 去除首尾空格
来源：http://xvp.sweek.top

SELECT TRIM(name) FROM users;
来源：http://cld.tanke756.top

[Q85] 数值取整
来源：http://oax.vqdsnc.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kcq.hcnkem.com

[Q86] 读取 JSON 字段
来源：http://yqj.andypj.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://leu.jinyuanbaomall.cn

[Q87] JSON 字段做条件
来源：http://mkb.xuetiantiany.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pab.wangshuangyany.cn

[Q88] 行转列（条件聚合）
来源：http://yge.shuidangran.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mzw.gaohongyu789.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://efp.dashuyun.cn

[Q89] 判断表是否存在
来源：http://ymo.daxiang520.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://chk.zhixingplan.top

[Q90] 生成序号列
来源：http://pcu.pycfn.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://atq.fehbvm.com

================================================================================
来源：http://ywq.xuanzx.com

R. Bash 专题
来源：http://txu.zhongyouzk.top

================================================================================
来源：http://qsu.yj20258.top

[R01] shebang 与严格模式
来源：http://ata.ctjpmb.com

#!/usr/bin/env bash
来源：http://jdi.gzhubu.top

set -euo pipefail
来源：http://hiu.yfazqb.com

[R02] 变量赋值与使用
来源：http://ygd.sweek.top

name="Tom"; echo "$name"
来源：http://iay.smart0.xyz

[R03] 只读变量
来源：http://qav.yfazqb.com

readonly PI=3.14
来源：http://uoj.yuxming.cn

[R04] 位置参数
来源：http://efc.nanxuanxn.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wrd.jianghu66.top

[R05] 参数默认值
来源：http://xiy.hongshengwenyu.top

name="${1:-default}"
来源：http://gxy.hesvh.cn

[R06] 判断命令是否存在
来源：http://nvu.redwolf501.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uld.gogol.net.cn

[R07] if 判断文件
来源：http://voe.shzxlz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bih.yvedp.cn

[R08] 数值比较
来源：http://fgk.svipenyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zxq.hnxiangtu.top

[R09] 字符串比较
来源：http://kim.epnwcf.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vis.shanyushiyangkeji.top

[R10] 正则匹配
来源：http://wca.fehbvm.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://owd.ydzc1.top

[R11] case 多分支
来源：http://cwl.316326.xyz

case "$1" in
来源：http://ocq.zhoulong.xyz

start) echo "启动" ;;
来源：http://heo.jianghu66.top

stop)  echo "停止" ;;
来源：http://hgy.jinyuanbaomall.cn

*)     echo "未知命令" ;;
来源：http://mhy.pycfn.com

esac
来源：http://rce.ydzc1.top

[R12] for 遍历文件
来源：http://kga.ydzc1.top

for f in *.txt; do echo "$f"; done
来源：http://sqe.nanxinkj.top

[R13] for 计数循环
来源：http://mvx.gzhubu.top

for i in {1..10}; do echo "$i"; done
来源：http://lsk.jinyuanbaomall.cn

[R14] C 风格 for
来源：http://hdo.52xcode.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vbw.yuxming.cn

[R15] while 逐行读文件
来源：http://azi.jinqigfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wxg.xuanzx.com

[R16] until 等待条件
来源：http://bty.kuanghao11.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wbk.jqgfzy.top

[R17] 数组定义与取值
来源：http://ucw.ydjk.org.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gik.fanxiaobao.xyz

[R18] 遍历数组
来源：http://xem.ywan-chungtsiang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fjr.dianchejie.cn

[R19] 数组长度
来源：http://elm.sxryk.cn

echo "${#arr[@]}"
来源：http://lnj.yuanzhike.top

[R20] 关联数组（字典）
来源：http://kbi.pengpengdd.cyou

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://opi.9152youxi.cn

[R21] 字符串长度
来源：http://evl.redwolf501.top

echo "${#s}"
来源：http://mxy.yfazqb.com

[R22] 截取子串
来源：http://ayj.yj20258.top

echo "${s:0:5}"
来源：http://ccq.c1oappe.top

[R23] 字符串替换
来源：http://iij.tian-w.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mfg.zhiwuduotai.top

[R24] 大小写转换
来源：http://tke.aizwys.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xfw.meibo888.top

[R25] 去后缀 / 去前缀
来源：http://lwb.daria6918.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://auj.jlsjyb.cn

[R26] 命令替换
来源：http://gjz.sysykeji.top

now=$(date +%F); echo "$now"
来源：http://vet.c1oappe.top

[R27] 算术展开
来源：http://fyb.snrcjt.cn

echo $((1 + 2 * 3))
来源：http://rsk.cheryme.top

[R28] 浮点运算
来源：http://uku.guowangkeji.top

echo "scale=2; 10/3" | bc
来源：http://ilr.ivvv.top

[R29] 定义函数
来源：http://vlf.hywenlv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://knv.jinqigufen.top

[R30] 函数返回状态码
来源：http://odx.haohaochexian.top

f() { return 0; }; f || echo "失败了"
来源：http://gjf.yongpay.top

[R31] 局部变量
来源：http://oqu.haohaochexian.top

f() { local x=1; echo "$x"; }
来源：http://apr.shzxlz.cn

[R32] 参数个数校验
来源：http://nuu.ydzc1.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rlb.cheryme.top

[R33] 捕获错误并提示行号
来源：http://hdb.dashuyun.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rvr.tanke756.top

[R34] 退出时清理
来源：http://nxl.shanyushiyangtech.top

trap 'rm -f "$tmp"' EXIT
来源：http://vqm.redwolf501.top

[R35] 后台执行并等待
来源：http://jnv.nwbrower.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wdr.ppjwa.cn

[R36] 并发执行多个任务
来源：http://flp.yj20258888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://csg.ppjwa.cn

[R37] 把输出赋给变量
来源：http://jkv.daria6918.cn

files=$(ls -1)
来源：http://muc.jianghu66.top

[R38] 管道串联
来源：http://yib.uphjek.com

cat a.txt | grep -i error | wc -l
来源：http://cog.sysykeji.top

[R39] 重定向标准输出与错误
来源：http://mvf.sjlbkw.cn

cmd > out.log 2>&1
来源：http://hzs.cheryme.top

[R40] 追加写日志
来源：http://tck.nanxinkj.top

echo "log" >> out.log
来源：http://etr.iojbl.cn

[R41] 丢弃输出
来源：http://pob.gaohongyu789.top

cmd >/dev/null 2>&1
来源：http://war.daria6918.cn

[R42] 输入重定向
来源：http://mvw.nwbrower.top

wc -l < a.txt
来源：http://wij.zhengqikj.top

[R43] 按名字查找文件
来源：http://iux.tanke756.top

find . -name "*.log" -type f
来源：http://vdc.cheryme.top

[R44] 按修改时间查找
来源：http://tob.yonumen.top

find . -mtime -7 -type f
来源：http://ixv.yj20258.top

[R45] 批量删除
来源：http://pts.chenjidiqi.icu

find . -name "*.tmp" -delete
来源：http://rjh.xuanzx.com

[R46] 递归替换文件内容
来源：http://dfh.cdnleiting.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sva.jlsjyb.cn

[R47] sed 单行替换
来源：http://guk.yj20258888.top

sed -i 's/foo/bar/g' a.txt
来源：http://ogx.tian-w.cn

[R48] awk 取指定列
来源：http://ibg.yangfankeji.com

awk '{print $1, $3}' a.txt
来源：http://xoq.yonumen.top

[R49] awk 带条件
来源：http://pnj.hcnkem.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qzv.jqgufenzy.top

[R50] awk 求和
来源：http://atf.dashuyun.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ccl.shangyingyoupin.top

[R51] 排序去重取前几
来源：http://xrx.shzxlz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mwn.9152youxi.cn

[R52] 统计行数
来源：http://xup.shangyingyoupin.top

wc -l a.txt
来源：http://mxi.cashguo.top

[R53] 查看文件头与实时尾
来源：http://gtq.nanxinkj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dkk.nanxuanxn.top

[R54] 比较两个文件
来源：http://wrr.c1oappe.top

diff a.txt b.txt
来源：http://fkz.kuanghao11.cn

[R55] 压缩与解压
来源：http://qxv.tarul.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xkf.cdnleiting.top

[R56] 远程拷贝
来源：http://bql.zhengqikj.top

scp file user@host:/path/
来源：http://qjy.cashguo.top

[R57] 远程执行命令
来源：http://nhj.quarkkingdee.top

ssh user@host 'uptime'
来源：http://qwx.c1oappe.top

[R58] 下载文件
来源：http://lan.dashuyun.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://njv.snrcjt.cn

[R59] 发 POST JSON
来源：http://ngm.tarul.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://klm.iojbl.cn

[R60] 只看 HTTP 状态码
来源：http://acr.zhijiandao.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ntl.zhengqikj.top

[R61] 磁盘占用
来源：http://hpm.52xcode.cn

df -h;  du -sh *
来源：http://isz.cdnleiting.top

[R62] 找最占空间的文件
来源：http://zjr.0kj1m.cn

du -ah . | sort -rh | head -10
来源：http://zgl.pycfn.com

[R63] 内存与进程
来源：http://ghm.fktsv.cn

free -h;  ps aux | grep nginx
来源：http://gix.316326.xyz

[R64] 结束进程
来源：http://yyz.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://myu.316326.xyz

[R65] 查看端口占用
来源：http://wrw.snrcjt.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qfz.hywenlv.cn

[R66] 定时任务
来源：http://oeo.hywenlv.cn

crontab -e;  crontab -l
来源：http://lro.fehbvm.com

[R67] 生成随机十六进制串
来源：http://psc.zycfv.cn

openssl rand -hex 16
来源：http://fli.gogol.net.cn

[R68] 计算文件校验值
来源：http://jzx.zhoulong.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://mrw.jqgufenzy.top

[R69] 生成随机密码
来源：http://jbp.9152youxi.cn

head -c 16 /dev/urandom | base64
来源：http://idi.aibaodan.cn

[R70] 时间戳与互转
来源：http://vgf.pycfn.com

date +%s;  date -d @1700000000
来源：http://dig.hnxiangtu.top

[R71] 日期格式化
来源：http://aby.tian-w.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dhi.ydzc1.top

[R72] 等待端口就绪
来源：http://yqr.jianghu66.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vyy.wangdashe.top

[R73] 分割大日志
来源：http://kji.birdmap.top

split -l 1000 big.log part_
来源：http://yxs.ctjpmb.com

[R74] 批量重命名
来源：http://jcv.gogol.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mun.hesvh.cn

[R75] 导出环境变量
来源：http://ttj.jinyuanbaomall.cn

export PATH="$HOME/bin:$PATH"
来源：http://uoq.meibo888.top

[R76] 使用临时文件
来源：http://ken.birdmap.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xub.pengpengdd.cyou

[R77] 读取用户输入
来源：http://izp.birdmap.top

read -rp "请输入: " ans
来源：http://gpu.yj20258.top

[R78] 交互式菜单
来源：http://cbw.andypj.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://exq.dianchejie.cn

[R79] 解析命令行选项
来源：http://beb.feifeiyinyue.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kbm.sufxvd.cn

[R80] 查看脚本执行耗时
来源：http://nvg.hesvh.cn

time ./run.sh
来源：http://hwq.xingfuxueyuan.xyz

================================================================================
来源：http://gws.xinyue.icu

S. C / C++ 专题
来源：http://yjw.wangshuangyany.cn

================================================================================
来源：http://uqi.smart0.xyz

[S01] C：Hello World
来源：http://dew.daria6918.cn

#include <stdio.h>
来源：http://eao.hcnkem.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://mhu.zhijiandao.cn

[S02] C：变量与格式化输出
来源：http://vna.birdmap.top

int a = 10; printf("%d\n", a);
来源：http://pdq.xylfe.cn

[S03] C：读入整数
来源：http://wrz.52xcode.cn

int x; scanf("%d", &x);
来源：http://wdn.yj202588.top

[S04] C：字符串复制
来源：http://wso.jianghu66.top

char dst[32]; strcpy(dst, "hi");
来源：http://fij.chenzaomai.com

[S05] C：字符串长度
来源：http://kpu.birdmap.top

strlen(s)
来源：http://azk.shanyushiyangkeji.top

[S06] C：字符串比较
来源：http://xat.vehdjk.com

strcmp(a, b) == 0
来源：http://ooz.gaohongyu789.top

[S07] C：数组遍历求和
来源：http://asf.yfazqb.com


<!-- 参考信息 -->