代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ktq.cashguo.top

[Q40] 交叉连接（笛卡尔积）
来源：http://utk.zycfv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tth.cheryme.top

[Q41] 多表连接
来源：http://hls.ybcxt.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://gfn.guannengcc.top

JOIN users u ON u.id = o.user_id
来源：http://jeg.hcnkem.com

JOIN products p ON p.id = o.product_id;
来源：http://rzz.zhongyouzk.top

[Q42] 连接条件附加过滤
来源：http://yfo.sweek.top

SELECT u.name, o.amount FROM users u
来源：http://zeg.yanxiufei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xiv.zhiwuduotai.top

[Q43] 标量子查询
来源：http://gow.shanyushiyangkeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://urm.fktsv.cn

[Q44] IN 子查询
来源：http://wqq.hfpthk.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://eww.hesvh.cn

[Q45] EXISTS 判断存在
来源：http://vvf.tian-w.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://luh.hysaishi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hvb.pengpengdd.cyou

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://egf.fanxiaobao.xyz

[Q47] 与平均值比较
来源：http://afj.tian-w.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://naz.52xcode.cn

[Q48] CTE 公用表表达式
来源：http://dvu.xingfuxueyuan.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vpx.yonumen.top

SELECT * FROM t WHERE c > 5;
来源：http://bqx.ydjk.org.cn

[Q49] 更新单行
来源：http://tbh.ydjk.org.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zop.smart0.xyz

[Q50] 批量更新
来源：http://rwi.sysykeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wgm.yvedp.cn

[Q51] 用子查询更新
来源：http://btw.ppjwa.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hvg.hammf.cn

[Q52] 删除指定行
来源：http://rmc.fehbvm.com

DELETE FROM users WHERE id = 10;
来源：http://hvb.xuetiantiany.cn

[Q53] 按条件删除
来源：http://uza.yueranfly.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ura.zhixingplan.top

[Q54] 清空表
来源：http://wpc.yangfankeji.com

TRUNCATE TABLE logs;
来源：http://msm.chenzaomai.com

[Q55] 排名（并列占位）
来源：http://jkf.hysaishi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zve.guannengcc.top

[Q56] 密集排名（并列不占位）
来源：http://ffk.zhijiandao.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dxw.yfazqb.com

[Q57] 行号
来源：http://riw.jyoumei.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ayc.iojbl.cn

[Q58] 累计求和
来源：http://smn.havefunace.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mkx.daxiang520.top

[Q59] 分组内累计
来源：http://xqc.fzhhl.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cmc.shanyushiyangtech.top

[Q60] 取上一行 / 下一行
来源：http://yuw.shzxlz.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ltk.iojbl.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bpn.c1oappe.top

[Q61] 移动平均
来源：http://sdz.zhiwuduotai.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ciz.yj20258.top

[Q62] 分组占比
来源：http://xrh.zdbjq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cro.gogol.net.cn

[Q63] 开启事务
来源：http://yzn.chenlongwang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zvv.redwolf501.top

[Q64] 提交事务
来源：http://idh.shzxlz.cn

COMMIT;
来源：http://uks.tarul.cn

[Q65] 回滚事务
来源：http://kec.hnxiangtu.top

ROLLBACK;
来源：http://pcm.xylfe.cn

[Q66] 行锁查询
来源：http://idm.ctjpmb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rgp.yj202588.top

[Q67] 设置隔离级别
来源：http://mum.xuanzx.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://afn.yanxiufei.cn

[Q68] 保存点
来源：http://lkw.shangyingyoupin.top

SAVEPOINT sp1;
来源：http://hlo.9152youxi.cn

ROLLBACK TO sp1;
来源：http://gms.shangyingyoupin.top

[Q69] 查看执行计划
来源：http://eya.tianlin.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oxh.kuanghao11.cn

[Q70] 更新统计信息
来源：http://yhp.sjlbkw.cn

ANALYZE TABLE users;
来源：http://edh.gotoacloud.top

[Q71] 查看建表语句
来源：http://dcb.svipenyu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bup.hnxiangtu.top

[Q72] 查看索引
来源：http://rvu.yj20258888.top

SHOW INDEX FROM users;
来源：http://vyi.cdnleiting.top

[Q73] 查看表状态
来源：http://rhe.jyoumei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rxr.sweek.top

[Q74] 强制使用索引
来源：http://fmr.gogol.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://odd.0kj1m.cn

[Q75] 日期格式化
来源：http://mut.yuanzhike.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tdf.fzhhl.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xka.jqgfzy.top

[Q76] 按天统计
来源：http://mxh.yj202588.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lbg.ydzc1.top

[Q77] 时间加减
来源：http://dao.zhijiandao.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qbc.zhiwuduotai.top

[Q78] 当前时间
来源：http://uoo.xylfe.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://emb.epnwcf.com

[Q79] 字符串拼接
来源：http://fdx.jiagoushi.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://clg.tian-w.cn

[Q80] 字符串截取
来源：http://kjh.ctjpmb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ufp.yuxming.cn

[Q81] 字符串替换
来源：http://dkv.zhixingplan.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yio.yueranfly.top

[Q82] 字符长度与字节长度
来源：http://hdk.quarkkingdee.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hxs.jqgufenzy.top

[Q83] 大小写转换
来源：http://rlo.zhaomingkeji.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xfq.xylfe.cn

[Q84] 去除首尾空格
来源：http://ozx.xziqi.cn

SELECT TRIM(name) FROM users;
来源：http://ozl.gaohongyu789.top

[Q85] 数值取整
来源：http://blm.dashuyun.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uyw.chenjidiqi.icu

[Q86] 读取 JSON 字段
来源：http://mfm.tianlin.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mxt.vehdjk.com

[Q87] JSON 字段做条件
来源：http://clv.meibo888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mjo.316326.xyz

[Q88] 行转列（条件聚合）
来源：http://svf.dashuyun.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wkn.haohaochexian.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vuh.gogol.net.cn

[Q89] 判断表是否存在
来源：http://mjk.pengpengdd.cyou

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pom.shangyingyoupin.top

[Q90] 生成序号列
来源：http://ped.tanke756.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dfk.ydzc1.top

================================================================================
来源：http://tqg.cqqwz.cn

R. Bash 专题
来源：http://xcw.0kj1m.cn

================================================================================
来源：http://pmn.dashuyun.cn

[R01] shebang 与严格模式
来源：http://kqx.gotoacloud.top

#!/usr/bin/env bash
来源：http://ibn.daria6918.cn

set -euo pipefail
来源：http://hsv.fengsongda.top

[R02] 变量赋值与使用
来源：http://gho.sxryk.cn

name="Tom"; echo "$name"
来源：http://mbh.sufxvd.cn

[R03] 只读变量
来源：http://zqe.xinyue.icu

readonly PI=3.14
来源：http://mde.quarkkingdee.top

[R04] 位置参数
来源：http://gar.chenzaomai.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tly.cheryme.top

[R05] 参数默认值
来源：http://jyj.jyoumei.cn

name="${1:-default}"
来源：http://dbb.316326.xyz

[R06] 判断命令是否存在
来源：http://ina.epnwcf.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://syq.yj20258888.top

[R07] if 判断文件
来源：http://fdh.jianghu66.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ifz.haohaochexian.top

[R08] 数值比较
来源：http://vhc.aizwys.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wkm.hesvh.cn

[R09] 字符串比较
来源：http://uol.hnqzz.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kwy.jiagoushi.top

[R10] 正则匹配
来源：http://rrw.cashguo.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ika.xingfuxueyuan.xyz

[R11] case 多分支
来源：http://hll.zhoulong.xyz

case "$1" in
来源：http://yzo.zhoulong.xyz

start) echo "启动" ;;
来源：http://xtm.xingfuxueyuan.xyz

stop)  echo "停止" ;;
来源：http://grs.gogol.net.cn

*)     echo "未知命令" ;;
来源：http://bar.ybcxt.top

esac
来源：http://dxk.redwolf501.top

[R12] for 遍历文件
来源：http://dxh.c1oappe.top

for f in *.txt; do echo "$f"; done
来源：http://bce.aizwys.cn

[R13] for 计数循环
来源：http://lay.gotoacloud.top

for i in {1..10}; do echo "$i"; done
来源：http://cip.chenzaomai.com

[R14] C 风格 for
来源：http://gsr.iojbl.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ity.pycfn.com

[R15] while 逐行读文件
来源：http://icm.chenlongwang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ebf.ywan-chungtsiang.top

[R16] until 等待条件
来源：http://uqw.hysaishi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uee.zycfv.cn

[R17] 数组定义与取值
来源：http://gmd.fzhhl.top

arr=(a b c); echo "${arr[0]}"
来源：http://lsr.bjfxy.top

[R18] 遍历数组
来源：http://hjc.dianchejie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://maa.hfpthk.cn

[R19] 数组长度
来源：http://eru.cheryme.top

echo "${#arr[@]}"
来源：http://ztc.hcnkem.com

[R20] 关联数组（字典）
来源：http://vwo.meibo888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mtr.zdbjq.cn

[R21] 字符串长度
来源：http://eul.smart0.xyz

echo "${#s}"
来源：http://lst.zdbjq.cn

[R22] 截取子串
来源：http://wcj.dianchejie.cn

echo "${s:0:5}"
来源：http://kxu.hammf.cn

[R23] 字符串替换
来源：http://ljx.jqgfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qag.tianlin.xyz

[R24] 大小写转换
来源：http://owu.feifeiyinyue.top

echo "${s^^}"; echo "${s,,}"
来源：http://fgh.jlsjyb.cn

[R25] 去后缀 / 去前缀
来源：http://qgp.yanxiufei.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tae.redwolf501.top

[R26] 命令替换
来源：http://uhl.zycfv.cn

now=$(date +%F); echo "$now"
来源：http://men.shanyushiyangkeji.top

[R27] 算术展开
来源：http://odl.gzhubu.top

echo $((1 + 2 * 3))
来源：http://kbm.zdqjudy.top

[R28] 浮点运算
来源：http://xwx.zdqjudy.top

echo "scale=2; 10/3" | bc
来源：http://suy.zdqjudy.top

[R29] 定义函数
来源：http://wje.chenzaomai.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wpb.shanyushiyangkeji.top

[R30] 函数返回状态码
来源：http://rrs.tian-w.cn

f() { return 0; }; f || echo "失败了"
来源：http://pqw.tanke756.top

[R31] 局部变量
来源：http://wkh.zycfv.cn

f() { local x=1; echo "$x"; }
来源：http://euu.uphjek.com

[R32] 参数个数校验
来源：http://vcj.gotoacloud.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ovf.jiagoushi.top

[R33] 捕获错误并提示行号
来源：http://hwp.vqdsnc.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xuu.jqgufenzy.top

[R34] 退出时清理
来源：http://hak.yuxming.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kqx.zhengqikj.top

[R35] 后台执行并等待
来源：http://eff.fengsongda.top

sleep 5 & pid=$!; wait "$pid"
来源：http://tyy.ppjwa.cn

[R36] 并发执行多个任务
来源：http://jzz.yueranfly.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sgd.guannengcc.top

[R37] 把输出赋给变量
来源：http://zkc.yj202588.top

files=$(ls -1)
来源：http://wju.mhx1999.top

[R38] 管道串联
来源：http://dtq.daxiang520.top

cat a.txt | grep -i error | wc -l
来源：http://tgo.yangfankeji.com

[R39] 重定向标准输出与错误
来源：http://ywo.birdmap.top

cmd > out.log 2>&1
来源：http://flj.daria6918.cn

[R40] 追加写日志
来源：http://too.ctjpmb.com

echo "log" >> out.log
来源：http://zvr.yfazqb.com

[R41] 丢弃输出
来源：http://ofg.yj202588.top

cmd >/dev/null 2>&1
来源：http://fqk.jinyuanbaomall.cn

[R42] 输入重定向
来源：http://vyv.c1oappe.top

wc -l < a.txt
来源：http://lys.yj202588.top

[R43] 按名字查找文件
来源：http://eed.hnxiangtu.top

find . -name "*.log" -type f
来源：http://qac.zhengqikj.top

[R44] 按修改时间查找
来源：http://umb.zycfv.cn

find . -mtime -7 -type f
来源：http://zwe.zhijiandao.cn

[R45] 批量删除
来源：http://vdk.uphjek.com

find . -name "*.tmp" -delete
来源：http://vbf.zhengqikj.top

[R46] 递归替换文件内容
来源：http://kpn.zycfv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xnf.svipenyu.cn

[R47] sed 单行替换
来源：http://dto.epnwcf.com

sed -i 's/foo/bar/g' a.txt
来源：http://aqd.bjfxy.top

[R48] awk 取指定列
来源：http://mwt.meibo888.top

awk '{print $1, $3}' a.txt
来源：http://juw.yangfankeji.com

[R49] awk 带条件
来源：http://pzz.fzhhl.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zui.jinqigfzy.top

[R50] awk 求和
来源：http://ajr.zdqjudy.top

awk '{s += $2} END {print s}' a.txt
来源：http://wpo.jianghu66.top

[R51] 排序去重取前几
来源：http://ofl.sxryk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bcb.fktsv.cn

[R52] 统计行数
来源：http://gdy.zhoulong.xyz

wc -l a.txt
来源：http://hxh.zhongyouzk.top

[R53] 查看文件头与实时尾
来源：http://bdw.ppjwa.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xgd.sjlbkw.cn

[R54] 比较两个文件
来源：http://ung.snrcjt.cn

diff a.txt b.txt
来源：http://csa.feifeiyinyue.top

[R55] 压缩与解压
来源：http://ewm.xinyue.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uzj.chenlongwang.top

[R56] 远程拷贝
来源：http://qui.gzhubu.top

scp file user@host:/path/
来源：http://zjg.fktsv.cn

[R57] 远程执行命令
来源：http://kxy.gotoacloud.top

ssh user@host 'uptime'
来源：http://mmb.nwbrower.top

[R58] 下载文件
来源：http://izu.shanyushiyangkeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zwk.shzxlz.cn

[R59] 发 POST JSON
来源：http://wmn.fktsv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uxc.yuxming.cn

[R60] 只看 HTTP 状态码
来源：http://rgx.pengpengdd.cyou

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qrf.yfazqb.com

[R61] 磁盘占用
来源：http://yuv.daxiang520.top

df -h;  du -sh *
来源：http://uam.bjfxy.top

[R62] 找最占空间的文件
来源：http://zhg.tianlin.xyz

du -ah . | sort -rh | head -10
来源：http://wve.hesvh.cn

[R63] 内存与进程
来源：http://yto.jinyuanbaomall.cn

free -h;  ps aux | grep nginx
来源：http://sgb.ehwqpu.com

[R64] 结束进程
来源：http://rvf.gotoacloud.top

kill -9 $(pgrep -f app.py)
来源：http://wny.yanxiufei.cn

[R65] 查看端口占用
来源：http://roa.zhoulong.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mxl.jlsjyb.cn

[R66] 定时任务
来源：http://bcf.uphjek.com

crontab -e;  crontab -l
来源：http://mfo.redwolf501.top

[R67] 生成随机十六进制串
来源：http://cat.guowangkeji.top

openssl rand -hex 16
来源：http://kuu.tianlin.xyz

[R68] 计算文件校验值
来源：http://pqn.pengpengdd.cyou

sha256sum a.txt;  md5sum a.txt
来源：http://piu.sxryk.cn

[R69] 生成随机密码
来源：http://czv.yfazqb.com

head -c 16 /dev/urandom | base64
来源：http://xub.xziqi.cn

[R70] 时间戳与互转
来源：http://vbm.yfazqb.com

date +%s;  date -d @1700000000
来源：http://whp.yj20258888.top

[R71] 日期格式化
来源：http://rvw.yj20258888.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qmk.jianghu66.top

[R72] 等待端口就绪
来源：http://feu.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://jqv.xuetiantiany.cn

[R73] 分割大日志
来源：http://pna.xuanzx.com

split -l 1000 big.log part_
来源：http://vcm.sxryk.cn

[R74] 批量重命名
来源：http://iav.chenjidiqi.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xot.316326.xyz

[R75] 导出环境变量
来源：http://jrw.ppjwa.cn

export PATH="$HOME/bin:$PATH"
来源：http://phf.yuxming.cn

[R76] 使用临时文件
来源：http://mpq.316326.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gng.yj20258.top

[R77] 读取用户输入
来源：http://isp.zhongyouzk.top

read -rp "请输入: " ans
来源：http://pca.gogol.net.cn

[R78] 交互式菜单
来源：http://aoc.zdbjq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tsu.cashguo.top

[R79] 解析命令行选项
来源：http://tpm.pycfn.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ufi.fanxiaobao.xyz

[R80] 查看脚本执行耗时
来源：http://owg.c1oappe.top

time ./run.sh
来源：http://sxw.shanyushiyangtech.top

================================================================================
来源：http://ord.hnqzz.top

S. C / C++ 专题
来源：http://dnc.yfazqb.com

================================================================================
来源：http://mge.zhaomingkeji.xyz

[S01] C：Hello World
来源：http://awb.yueranfly.top

#include <stdio.h>
来源：http://cfl.zhongyouzk.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://cbs.pengpengdd.cyou

[S02] C：变量与格式化输出
来源：http://gbl.gaohongyu789.top

int a = 10; printf("%d\n", a);
来源：http://jpe.cucudq.cn

[S03] C：读入整数
来源：http://afe.chenlongwang.top

int x; scanf("%d", &x);
来源：http://ttt.jinghuilouyu.cn

[S04] C：字符串复制
来源：http://cnm.zhengqikj.top

char dst[32]; strcpy(dst, "hi");
来源：http://fte.chenjidiqi.icu

[S05] C：字符串长度
来源：http://pbg.jinyuanbaomall.cn

strlen(s)
来源：http://snb.epnwcf.com

[S06] C：字符串比较
来源：http://hre.jqgfzy.top

strcmp(a, b) == 0
来源：http://vyl.shanyushiyangkeji.top

[S07] C：数组遍历求和
来源：http://iro.jinqigufen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lpe.hesvh.cn

[S08] C：动态内存分配与释放
来源：http://ank.jinqigfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://scr.dianchejie.cn

[S09] C：结构体定义与初始化
来源：http://xyd.wangdashe.top


<!-- 参考信息 -->