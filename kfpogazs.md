代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://hld.birdmap.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jnw.yuxming.cn

[Q39] 自连接（查上下级）
来源：http://byp.iojbl.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zna.zdbjq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oeb.0kj1m.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xij.0kj1m.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zyt.yvedp.cn

[Q41] 多表连接
来源：http://cyr.gzhubu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://vdw.sufxvd.cn

JOIN users u ON u.id = o.user_id
来源：http://jjl.pycfn.com

JOIN products p ON p.id = o.product_id;
来源：http://lbj.yangfankeji.com

[Q42] 连接条件附加过滤
来源：http://rbh.xinyue.icu

SELECT u.name, o.amount FROM users u
来源：http://mav.tian-w.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jaz.birdmap.top

[Q43] 标量子查询
来源：http://myc.cheryme.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://inu.tianlin.xyz

[Q44] IN 子查询
来源：http://gpd.zhoulong.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fmn.iojbl.cn

[Q45] EXISTS 判断存在
来源：http://qqd.ehwqpu.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wav.ywan-chungtsiang.top

[Q46] NOT EXISTS 判断不存在
来源：http://osi.9152youxi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fdv.guowangkeji.top

[Q47] 与平均值比较
来源：http://ajb.xziqi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fna.xuetiantiany.cn

[Q48] CTE 公用表表达式
来源：http://wyp.aibaodan.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pvr.jinqigufen.top

SELECT * FROM t WHERE c > 5;
来源：http://yuv.tanke756.top

[Q49] 更新单行
来源：http://cim.gzhubu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kki.daria6918.cn

[Q50] 批量更新
来源：http://bhc.fzhhl.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xxh.zdbjq.cn

[Q51] 用子查询更新
来源：http://rsw.yj20258.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vaw.sweek.top

[Q52] 删除指定行
来源：http://uns.chenlongwang.top

DELETE FROM users WHERE id = 10;
来源：http://oap.fehbvm.com

[Q53] 按条件删除
来源：http://atn.ctjpmb.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://niz.zhoulong.xyz

[Q54] 清空表
来源：http://ocs.tian-w.cn

TRUNCATE TABLE logs;
来源：http://ibw.yj202588.top

[Q55] 排名（并列占位）
来源：http://sbs.jinyuanbaomall.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bed.hongshengwenyu.top

[Q56] 密集排名（并列不占位）
来源：http://tuc.yuxming.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://aoh.gaohongyu789.top

[Q57] 行号
来源：http://ant.quarkkingdee.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pgo.ivvv.top

[Q58] 累计求和
来源：http://uxk.jinqigfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://isa.nwbrower.top

[Q59] 分组内累计
来源：http://rzo.shanyushiyangtech.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ntx.yvedp.cn

[Q60] 取上一行 / 下一行
来源：http://mez.haohaochexian.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bop.zhixingplan.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://btt.feifeiyinyue.top

[Q61] 移动平均
来源：http://xko.vqdsnc.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://llh.9152youxi.cn

[Q62] 分组占比
来源：http://eue.shanyushiyangtech.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://aqo.cheryme.top

[Q63] 开启事务
来源：http://lik.hammf.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://byd.nwbrower.top

[Q64] 提交事务
来源：http://nfx.aibaodan.cn

COMMIT;
来源：http://iwa.xylfe.cn

[Q65] 回滚事务
来源：http://fvu.chenjidiqi.icu

ROLLBACK;
来源：http://iyf.yj20258.top

[Q66] 行锁查询
来源：http://rie.quarkkingdee.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://knt.gzhubu.top

[Q67] 设置隔离级别
来源：http://lcu.gzhubu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vvf.yfazqb.com

[Q68] 保存点
来源：http://nmn.tianlin.xyz

SAVEPOINT sp1;
来源：http://tza.zdbjq.cn

ROLLBACK TO sp1;
来源：http://wlr.nanxinkj.top

[Q69] 查看执行计划
来源：http://pjj.shanyushiyangkeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xmd.jyoumei.cn

[Q70] 更新统计信息
来源：http://yiv.ppjwa.cn

ANALYZE TABLE users;
来源：http://lcy.ehwqpu.com

[Q71] 查看建表语句
来源：http://qih.andypj.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sep.chenzaomai.com

[Q72] 查看索引
来源：http://cqj.cqqwz.cn

SHOW INDEX FROM users;
来源：http://yvp.yuxming.cn

[Q73] 查看表状态
来源：http://hsm.fanxiaobao.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://xzf.316326.xyz

[Q74] 强制使用索引
来源：http://hvn.guannengcc.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xam.birdmap.top

[Q75] 日期格式化
来源：http://irx.cucudq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xbu.sufxvd.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vxo.shzxlz.cn

[Q76] 按天统计
来源：http://yed.hysaishi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zrb.aibaodan.cn

[Q77] 时间加减
来源：http://cxb.jqgufenzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ami.mhx1999.top

[Q78] 当前时间
来源：http://lqb.xziqi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://abd.jiagoushi.top

[Q79] 字符串拼接
来源：http://kvf.ivvv.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zkt.chenlongwang.top

[Q80] 字符串截取
来源：http://nvq.jqgufenzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://atw.hcnkem.com

[Q81] 字符串替换
来源：http://cyx.smart0.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ilv.ybcxt.top

[Q82] 字符长度与字节长度
来源：http://wjb.ehwqpu.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ztf.yuanzhike.top

[Q83] 大小写转换
来源：http://gmb.gaohongyu789.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yly.hongshengwenyu.top

[Q84] 去除首尾空格
来源：http://fle.jinyuanbaomall.cn

SELECT TRIM(name) FROM users;
来源：http://emq.shanyushiyangtech.top

[Q85] 数值取整
来源：http://dhg.xuetiantiany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zfr.zdqjudy.top

[Q86] 读取 JSON 字段
来源：http://qim.fktsv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://axg.ydjk.org.cn

[Q87] JSON 字段做条件
来源：http://fvm.ywan-chungtsiang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rbz.ehwqpu.com

[Q88] 行转列（条件聚合）
来源：http://dbo.316326.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mqe.dashuyun.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uer.tian-w.cn

[Q89] 判断表是否存在
来源：http://uiq.c1oappe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qlx.jlsjyb.cn

[Q90] 生成序号列
来源：http://xvw.fanxiaobao.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wde.xingfuxueyuan.xyz

================================================================================
来源：http://stb.zhixingplan.top

R. Bash 专题
来源：http://zhw.jqgfzy.top

================================================================================
来源：http://ykl.ivvv.top

[R01] shebang 与严格模式
来源：http://lvc.pycfn.com

#!/usr/bin/env bash
来源：http://zll.jinqigufen.top

set -euo pipefail
来源：http://ugt.meibo888.top

[R02] 变量赋值与使用
来源：http://kmx.zhongyouzk.top

name="Tom"; echo "$name"
来源：http://xze.cheryme.top

[R03] 只读变量
来源：http://dnb.yuxming.cn

readonly PI=3.14
来源：http://yxz.sweek.top

[R04] 位置参数
来源：http://lfm.daxiang520.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zgb.ivvv.top

[R05] 参数默认值
来源：http://xiq.pengpengdd.cyou

name="${1:-default}"
来源：http://ami.yfazqb.com

[R06] 判断命令是否存在
来源：http://lbt.cdnleiting.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wds.gogol.net.cn

[R07] if 判断文件
来源：http://kgy.ydjk.org.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://azw.zycfv.cn

[R08] 数值比较
来源：http://nqy.uphjek.com

if (( a > b )); then echo "a 更大"; fi
来源：http://oer.ivvv.top

[R09] 字符串比较
来源：http://ioy.zdbjq.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wmh.hnqzz.top

[R10] 正则匹配
来源：http://djw.xuetiantiany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bex.uphjek.com

[R11] case 多分支
来源：http://zdr.daria6918.cn

case "$1" in
来源：http://jqy.guowangkeji.top

start) echo "启动" ;;
来源：http://rxh.nanxuanxn.top

stop)  echo "停止" ;;
来源：http://ztu.hnxiangtu.top

*)     echo "未知命令" ;;
来源：http://etr.yueranfly.top

esac
来源：http://imj.9152youxi.cn

[R12] for 遍历文件
来源：http://drt.chenlongwang.top

for f in *.txt; do echo "$f"; done
来源：http://cri.zhongyouzk.top

[R13] for 计数循环
来源：http://pwg.pengpengdd.cyou

for i in {1..10}; do echo "$i"; done
来源：http://hsl.jlsjyb.cn

[R14] C 风格 for
来源：http://twe.zhongyouzk.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qzv.jinqigufen.top

[R15] while 逐行读文件
来源：http://npz.xuanzx.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pzh.yj202588.top

[R16] until 等待条件
来源：http://wdq.zhongyouzk.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oas.gaohongyu789.top

[R17] 数组定义与取值
来源：http://dhs.jianghu66.top

arr=(a b c); echo "${arr[0]}"
来源：http://elr.yanxiufei.cn

[R18] 遍历数组
来源：http://jlk.yj20258888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jbs.jianghu66.top

[R19] 数组长度
来源：http://dij.shangyingyoupin.top

echo "${#arr[@]}"
来源：http://ifc.tarul.cn

[R20] 关联数组（字典）
来源：http://urw.jinqigfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eeu.redwolf501.top

[R21] 字符串长度
来源：http://vqy.fktsv.cn

echo "${#s}"
来源：http://uii.mhx1999.top

[R22] 截取子串
来源：http://uow.snrcjt.cn

echo "${s:0:5}"
来源：http://iql.hnxiangtu.top

[R23] 字符串替换
来源：http://rpk.wangshuangyany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jvd.gotoacloud.top

[R24] 大小写转换
来源：http://wlj.fengsongda.top

echo "${s^^}"; echo "${s,,}"
来源：http://gcr.hnqzz.top

[R25] 去后缀 / 去前缀
来源：http://gvx.guowangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fkv.jqgufenzy.top

[R26] 命令替换
来源：http://gmk.sweek.top

now=$(date +%F); echo "$now"
来源：http://mbf.yj20258888.top

[R27] 算术展开
来源：http://nsl.cqqwz.cn

echo $((1 + 2 * 3))
来源：http://fvk.uphjek.com

[R28] 浮点运算
来源：http://imw.zycfv.cn

echo "scale=2; 10/3" | bc
来源：http://cik.tarul.cn

[R29] 定义函数
来源：http://fod.sxryk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fhj.xziqi.cn

[R30] 函数返回状态码
来源：http://dhf.yfazqb.com

f() { return 0; }; f || echo "失败了"
来源：http://cwr.fktsv.cn

[R31] 局部变量
来源：http://xgb.fehbvm.com

f() { local x=1; echo "$x"; }
来源：http://mak.dianchejie.cn

[R32] 参数个数校验
来源：http://hfe.fzhhl.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wbl.meibo888.top

[R33] 捕获错误并提示行号
来源：http://gkt.sysykeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tbl.hywenlv.cn

[R34] 退出时清理
来源：http://aag.ydjk.org.cn

trap 'rm -f "$tmp"' EXIT
来源：http://voo.yfazqb.com

[R35] 后台执行并等待
来源：http://znr.ydjk.org.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://irs.hcnkem.com

[R36] 并发执行多个任务
来源：http://xwq.sweek.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zvj.hywenlv.cn

[R37] 把输出赋给变量
来源：http://paa.shuidangran.top

files=$(ls -1)
来源：http://qed.hongshengwenyu.top

[R38] 管道串联
来源：http://bsu.xylfe.cn

cat a.txt | grep -i error | wc -l
来源：http://bvo.wangdashe.top

[R39] 重定向标准输出与错误
来源：http://xyv.c1oappe.top

cmd > out.log 2>&1
来源：http://ntd.xylfe.cn

[R40] 追加写日志
来源：http://cpf.smart0.xyz

echo "log" >> out.log
来源：http://chk.yuxming.cn

[R41] 丢弃输出
来源：http://peb.yj202588.top

cmd >/dev/null 2>&1
来源：http://orb.chenzaomai.com

[R42] 输入重定向
来源：http://pgx.guowangkeji.top

wc -l < a.txt
来源：http://otk.birdmap.top

[R43] 按名字查找文件
来源：http://ixb.jyoumei.cn

find . -name "*.log" -type f
来源：http://eei.xingfuxueyuan.xyz

[R44] 按修改时间查找
来源：http://sdz.xingfuxueyuan.xyz

find . -mtime -7 -type f
来源：http://xjk.pycfn.com

[R45] 批量删除
来源：http://mex.birdmap.top

find . -name "*.tmp" -delete
来源：http://omf.meibo888.top

[R46] 递归替换文件内容
来源：http://wem.tianlin.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xpt.cdnleiting.top

[R47] sed 单行替换
来源：http://epd.cdnleiting.top

sed -i 's/foo/bar/g' a.txt
来源：http://cft.tanke756.top

[R48] awk 取指定列
来源：http://evw.gogol.net.cn

awk '{print $1, $3}' a.txt
来源：http://abv.yanxiufei.cn

[R49] awk 带条件
来源：http://ybr.mhx1999.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ist.aibaodan.cn

[R50] awk 求和
来源：http://pky.zhengqikj.top

awk '{s += $2} END {print s}' a.txt
来源：http://nxr.ybcxt.top

[R51] 排序去重取前几
来源：http://epw.zhengqikj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://stw.uphjek.com

[R52] 统计行数
来源：http://udp.ybcxt.top

wc -l a.txt
来源：http://umv.daxiang520.top

[R53] 查看文件头与实时尾
来源：http://brp.0kj1m.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rux.fktsv.cn

[R54] 比较两个文件
来源：http://qbd.sweek.top

diff a.txt b.txt
来源：http://qdj.shangyingyoupin.top

[R55] 压缩与解压
来源：http://obv.xingfuxueyuan.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wfg.hfpthk.cn

[R56] 远程拷贝
来源：http://snz.zhiwuduotai.top

scp file user@host:/path/
来源：http://tue.zhaomingkeji.xyz

[R57] 远程执行命令
来源：http://inz.ppjwa.cn

ssh user@host 'uptime'
来源：http://fkj.shanyushiyangtech.top

[R58] 下载文件
来源：http://heb.yj20258888.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ito.hfpthk.cn

[R59] 发 POST JSON
来源：http://noh.yvedp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nzi.yangfankeji.com

[R60] 只看 HTTP 状态码
来源：http://vtn.shangyingyoupin.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sxd.chenlongwang.top

[R61] 磁盘占用
来源：http://gub.haohaochexian.top

df -h;  du -sh *
来源：http://zcz.pengpengdd.cyou

[R62] 找最占空间的文件
来源：http://pgr.xuetiantiany.cn

du -ah . | sort -rh | head -10
来源：http://bhs.316326.xyz

[R63] 内存与进程
来源：http://fem.wangshuangyany.cn

free -h;  ps aux | grep nginx
来源：http://zvj.sysykeji.top

[R64] 结束进程
来源：http://ami.shuidangran.top

kill -9 $(pgrep -f app.py)
来源：http://hci.sxryk.cn

[R65] 查看端口占用
来源：http://zpe.jianghu66.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gzw.xingfuxueyuan.xyz

[R66] 定时任务
来源：http://gmv.havefunace.top

crontab -e;  crontab -l
来源：http://iso.feifeiyinyue.top

[R67] 生成随机十六进制串
来源：http://ujy.fehbvm.com

openssl rand -hex 16
来源：http://mei.jyoumei.cn

[R68] 计算文件校验值
来源：http://rri.hcnkem.com

sha256sum a.txt;  md5sum a.txt
来源：http://mhd.xylfe.cn

[R69] 生成随机密码
来源：http://yib.fengsongda.top

head -c 16 /dev/urandom | base64
来源：http://ftj.pengpengdd.cyou

[R70] 时间戳与互转
来源：http://xsl.tianlin.xyz

date +%s;  date -d @1700000000
来源：http://euh.kuanghao11.cn

[R71] 日期格式化
来源：http://ltb.hongshengwenyu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://fkr.cucudq.cn

[R72] 等待端口就绪
来源：http://aiq.cdnleiting.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dxp.zhiwuduotai.top

[R73] 分割大日志
来源：http://ots.yj20258888.top

split -l 1000 big.log part_
来源：http://rvw.yj20258.top

[R74] 批量重命名
来源：http://ynr.hnxiangtu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wya.yuanzhike.top

[R75] 导出环境变量
来源：http://gok.epnwcf.com

export PATH="$HOME/bin:$PATH"
来源：http://bfv.daria6918.cn

[R76] 使用临时文件
来源：http://clk.kuanghao11.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://slx.andypj.xyz

[R77] 读取用户输入
来源：http://tmd.yfazqb.com

read -rp "请输入: " ans
来源：http://wxp.yonumen.top

[R78] 交互式菜单
来源：http://voi.snrcjt.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xqm.sjlbkw.cn

[R79] 解析命令行选项
来源：http://vdm.tian-w.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dkp.jinyuanbaomall.cn

[R80] 查看脚本执行耗时
来源：http://vpc.guannengcc.top

time ./run.sh
来源：http://pve.yongpay.top

================================================================================
来源：http://nsv.smart0.xyz

S. C / C++ 专题
来源：http://upn.hnxiangtu.top

================================================================================
来源：http://euz.hcnkem.com

[S01] C：Hello World
来源：http://riq.zdbjq.cn

#include <stdio.h>
来源：http://iib.gotoacloud.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bji.zycfv.cn

[S02] C：变量与格式化输出
来源：http://qgl.zhiwuduotai.top

int a = 10; printf("%d\n", a);
来源：http://vuo.sufxvd.cn

[S03] C：读入整数
来源：http://rum.guannengcc.top

int x; scanf("%d", &x);
来源：http://stk.cheryme.top

[S04] C：字符串复制
来源：http://chv.c1oappe.top

char dst[32]; strcpy(dst, "hi");
来源：http://mjv.ctjpmb.com

[S05] C：字符串长度
来源：http://spq.yfazqb.com

strlen(s)
来源：http://tow.ehwqpu.com

[S06] C：字符串比较
来源：http://pkx.birdmap.top

strcmp(a, b) == 0
来源：http://iec.yuxming.cn

[S07] C：数组遍历求和
来源：http://cug.yvedp.cn


<!-- 参考信息 -->