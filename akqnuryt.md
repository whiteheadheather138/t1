代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://dqf.fanxiaobao.xyz

JOIN users u ON u.id = o.user_id
来源：http://qtz.52xcode.cn

JOIN products p ON p.id = o.product_id;
来源：http://hcp.ppjwa.cn

[Q42] 连接条件附加过滤
来源：http://etv.yuanzhike.top

SELECT u.name, o.amount FROM users u
来源：http://btv.epnwcf.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lox.yangfankeji.com

[Q43] 标量子查询
来源：http://kve.svipenyu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gte.yongpay.top

[Q44] IN 子查询
来源：http://ffs.jianghu66.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hbb.shuidangran.top

[Q45] EXISTS 判断存在
来源：http://lwx.guowangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mup.0kj1m.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nyu.cdnleiting.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mjr.52xcode.cn

[Q47] 与平均值比较
来源：http://xjt.jiagoushi.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ntk.shangyingyoupin.top

[Q48] CTE 公用表表达式
来源：http://kbu.yj202588.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://srv.quarkkingdee.top

SELECT * FROM t WHERE c > 5;
来源：http://aqc.andypj.xyz

[Q49] 更新单行
来源：http://das.yj20258888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wjg.smart0.xyz

[Q50] 批量更新
来源：http://bky.ydzc1.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rar.chenzaomai.com

[Q51] 用子查询更新
来源：http://cas.shuidangran.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vus.zhengqikj.top

[Q52] 删除指定行
来源：http://jqa.hysaishi.cn

DELETE FROM users WHERE id = 10;
来源：http://twt.yj202588.top

[Q53] 按条件删除
来源：http://ikh.hesvh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xxr.cucudq.cn

[Q54] 清空表
来源：http://qmh.yanxiufei.cn

TRUNCATE TABLE logs;
来源：http://mph.hysaishi.cn

[Q55] 排名（并列占位）
来源：http://iuu.yonumen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vwv.daria6918.cn

[Q56] 密集排名（并列不占位）
来源：http://lst.guannengcc.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lxj.tanke756.top

[Q57] 行号
来源：http://kop.316326.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lra.shanyushiyangtech.top

[Q58] 累计求和
来源：http://lzt.ydzc1.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ocs.ehwqpu.com

[Q59] 分组内累计
来源：http://rrl.bjfxy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://esh.jyoumei.cn

[Q60] 取上一行 / 下一行
来源：http://zlo.c1oappe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vej.zhixingplan.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tvb.fktsv.cn

[Q61] 移动平均
来源：http://usn.jlsjyb.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iya.c1oappe.top

[Q62] 分组占比
来源：http://bgr.zycfv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://azp.fzhhl.top

[Q63] 开启事务
来源：http://hyv.zdqjudy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://xwx.hfpthk.cn

[Q64] 提交事务
来源：http://ayj.zdqjudy.top

COMMIT;
来源：http://ira.mhx1999.top

[Q65] 回滚事务
来源：http://lwa.gaohongyu789.top

ROLLBACK;
来源：http://mvm.yangfankeji.com

[Q66] 行锁查询
来源：http://edj.hnxiangtu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wwc.yongpay.top

[Q67] 设置隔离级别
来源：http://ewy.gaohongyu789.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hti.hysaishi.cn

[Q68] 保存点
来源：http://klu.fzhhl.top

SAVEPOINT sp1;
来源：http://cht.jinghuilouyu.cn

ROLLBACK TO sp1;
来源：http://zyz.316326.xyz

[Q69] 查看执行计划
来源：http://lzq.uphjek.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://axg.chenjidiqi.icu

[Q70] 更新统计信息
来源：http://dju.xuanzx.com

ANALYZE TABLE users;
来源：http://dvu.daxiang520.top

[Q71] 查看建表语句
来源：http://rxp.redwolf501.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ueq.havefunace.top

[Q72] 查看索引
来源：http://tqo.nanxinkj.top

SHOW INDEX FROM users;
来源：http://nda.havefunace.top

[Q73] 查看表状态
来源：http://xbj.sjlbkw.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bqy.hnxiangtu.top

[Q74] 强制使用索引
来源：http://uka.wangdashe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zuj.xuetiantiany.cn

[Q75] 日期格式化
来源：http://ayp.gotoacloud.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://grb.fehbvm.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://amg.zhaomingkeji.xyz

[Q76] 按天统计
来源：http://zrs.shzxlz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vjl.xinyue.icu

[Q77] 时间加减
来源：http://ury.smart0.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fbs.jiagoushi.top

[Q78] 当前时间
来源：http://paj.havefunace.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hnp.pycfn.com

[Q79] 字符串拼接
来源：http://bni.zdqjudy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://enc.jinqigfzy.top

[Q80] 字符串截取
来源：http://hhv.xziqi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yiq.zhengqikj.top

[Q81] 字符串替换
来源：http://lff.nanxuanxn.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kni.hesvh.cn

[Q82] 字符长度与字节长度
来源：http://fuh.pycfn.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kvy.cashguo.top

[Q83] 大小写转换
来源：http://lgb.fzhhl.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dyp.fanxiaobao.xyz

[Q84] 去除首尾空格
来源：http://cqt.aizwys.cn

SELECT TRIM(name) FROM users;
来源：http://gyd.fehbvm.com

[Q85] 数值取整
来源：http://hzj.shanyushiyangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yht.birdmap.top

[Q86] 读取 JSON 字段
来源：http://htv.shzxlz.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://quu.hesvh.cn

[Q87] JSON 字段做条件
来源：http://czg.yj20258888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cld.sufxvd.cn

[Q88] 行转列（条件聚合）
来源：http://lje.dashuyun.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mbm.yuanzhike.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cxh.c1oappe.top

[Q89] 判断表是否存在
来源：http://ico.sweek.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bfr.haohaochexian.top

[Q90] 生成序号列
来源：http://hut.feifeiyinyue.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tcj.aibaodan.cn

================================================================================
来源：http://nyn.yonumen.top

R. Bash 专题
来源：http://xbb.tanke756.top

================================================================================
来源：http://xqz.fzhhl.top

[R01] shebang 与严格模式
来源：http://gok.tianlin.xyz

#!/usr/bin/env bash
来源：http://ykq.bjfxy.top

set -euo pipefail
来源：http://vxf.316326.xyz

[R02] 变量赋值与使用
来源：http://rnq.jinqigfzy.top

name="Tom"; echo "$name"
来源：http://gqv.zhoulong.xyz

[R03] 只读变量
来源：http://abz.fzhhl.top

readonly PI=3.14
来源：http://yok.birdmap.top

[R04] 位置参数
来源：http://fop.pycfn.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://evt.zycfv.cn

[R05] 参数默认值
来源：http://dgs.chenzaomai.com

name="${1:-default}"
来源：http://zue.jinghuilouyu.cn

[R06] 判断命令是否存在
来源：http://oze.ydjk.org.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dfv.yueranfly.top

[R07] if 判断文件
来源：http://xxf.chenjidiqi.icu

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rkq.gogol.net.cn

[R08] 数值比较
来源：http://wqr.ydzc1.top

if (( a > b )); then echo "a 更大"; fi
来源：http://znw.jqgufenzy.top

[R09] 字符串比较
来源：http://oao.sysykeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gpm.hfpthk.cn

[R10] 正则匹配
来源：http://wsr.hongshengwenyu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sas.sjlbkw.cn

[R11] case 多分支
来源：http://ujs.ydzc1.top

case "$1" in
来源：http://axp.yj202588.top

start) echo "启动" ;;
来源：http://lci.9152youxi.cn

stop)  echo "停止" ;;
来源：http://blm.quarkkingdee.top

*)     echo "未知命令" ;;
来源：http://zbw.yfazqb.com

esac
来源：http://ynp.yuxming.cn

[R12] for 遍历文件
来源：http://zwr.yj202588.top

for f in *.txt; do echo "$f"; done
来源：http://mrg.jinyuanbaomall.cn

[R13] for 计数循环
来源：http://isc.sysykeji.top

for i in {1..10}; do echo "$i"; done
来源：http://qxd.birdmap.top

[R14] C 风格 for
来源：http://yqu.hesvh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://afe.vqdsnc.cn

[R15] while 逐行读文件
来源：http://lht.yvedp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zha.chenzaomai.com

[R16] until 等待条件
来源：http://moq.cucudq.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ucb.hesvh.cn

[R17] 数组定义与取值
来源：http://dqk.shzxlz.cn

arr=(a b c); echo "${arr[0]}"
来源：http://olx.aizwys.cn

[R18] 遍历数组
来源：http://rtg.andypj.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gyz.chenzaomai.com

[R19] 数组长度
来源：http://gri.xziqi.cn

echo "${#arr[@]}"
来源：http://bic.hfpthk.cn

[R20] 关联数组（字典）
来源：http://bcj.chenlongwang.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uoi.xuanzx.com

[R21] 字符串长度
来源：http://nqe.yj20258888.top

echo "${#s}"
来源：http://ubq.ydzc1.top

[R22] 截取子串
来源：http://cif.sxryk.cn

echo "${s:0:5}"
来源：http://tuu.cashguo.top

[R23] 字符串替换
来源：http://mwg.svipenyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mzb.ydjk.org.cn

[R24] 大小写转换
来源：http://zmc.gzhubu.top

echo "${s^^}"; echo "${s,,}"
来源：http://fzs.jinqigufen.top

[R25] 去后缀 / 去前缀
来源：http://atk.hywenlv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://epk.zhiwuduotai.top

[R26] 命令替换
来源：http://ump.sjlbkw.cn

now=$(date +%F); echo "$now"
来源：http://gwq.mhx1999.top

[R27] 算术展开
来源：http://oey.yonumen.top

echo $((1 + 2 * 3))
来源：http://yzo.shanyushiyangtech.top

[R28] 浮点运算
来源：http://sql.gzhubu.top

echo "scale=2; 10/3" | bc
来源：http://kqv.yongpay.top

[R29] 定义函数
来源：http://nba.yj202588.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uzy.birdmap.top

[R30] 函数返回状态码
来源：http://xdi.guowangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://qhs.gotoacloud.top

[R31] 局部变量
来源：http://anz.chenzaomai.com

f() { local x=1; echo "$x"; }
来源：http://kla.cdnleiting.top

[R32] 参数个数校验
来源：http://zbd.xziqi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gqg.nanxinkj.top

[R33] 捕获错误并提示行号
来源：http://ogh.haohaochexian.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dpt.hysaishi.cn

[R34] 退出时清理
来源：http://mlw.redwolf501.top

trap 'rm -f "$tmp"' EXIT
来源：http://tbg.zdqjudy.top

[R35] 后台执行并等待
来源：http://tnb.sysykeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dbu.wangdashe.top

[R36] 并发执行多个任务
来源：http://urn.aibaodan.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zlb.xingfuxueyuan.xyz

[R37] 把输出赋给变量
来源：http://lct.yuxming.cn

files=$(ls -1)
来源：http://oti.0kj1m.cn

[R38] 管道串联
来源：http://eeo.havefunace.top

cat a.txt | grep -i error | wc -l
来源：http://upp.cashguo.top

[R39] 重定向标准输出与错误
来源：http://zfy.ppjwa.cn

cmd > out.log 2>&1
来源：http://lhl.snrcjt.cn

[R40] 追加写日志
来源：http://rqu.zhijiandao.cn

echo "log" >> out.log
来源：http://nzz.shanyushiyangtech.top

[R41] 丢弃输出
来源：http://qir.shzxlz.cn

cmd >/dev/null 2>&1
来源：http://com.bbcook.cn

[R42] 输入重定向
来源：http://bgq.zdbjq.cn

wc -l < a.txt
来源：http://rks.vehdjk.com

[R43] 按名字查找文件
来源：http://gxe.jqgfzy.top

find . -name "*.log" -type f
来源：http://rco.aizwys.cn

[R44] 按修改时间查找
来源：http://hzr.fanxiaobao.xyz

find . -mtime -7 -type f
来源：http://tmp.zdbjq.cn

[R45] 批量删除
来源：http://ymt.xuetiantiany.cn

find . -name "*.tmp" -delete
来源：http://meg.hongshengwenyu.top

[R46] 递归替换文件内容
来源：http://pve.mhx1999.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pvp.9152youxi.cn

[R47] sed 单行替换
来源：http://ukf.ppjwa.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mjd.gogol.net.cn

[R48] awk 取指定列
来源：http://xed.shzxlz.cn

awk '{print $1, $3}' a.txt
来源：http://mcx.hesvh.cn

[R49] awk 带条件
来源：http://ohc.vqdsnc.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bdw.jlsjyb.cn

[R50] awk 求和
来源：http://mpx.pycfn.com

awk '{s += $2} END {print s}' a.txt
来源：http://xhn.yfazqb.com

[R51] 排序去重取前几
来源：http://oui.xylfe.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ztg.yuanzhike.top

[R52] 统计行数
来源：http://gej.sjlbkw.cn

wc -l a.txt
来源：http://kfn.hcnkem.com

[R53] 查看文件头与实时尾
来源：http://fkd.jinqigufen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pgn.andypj.xyz

[R54] 比较两个文件
来源：http://snd.316326.xyz

diff a.txt b.txt
来源：http://mrt.snrcjt.cn

[R55] 压缩与解压
来源：http://jpx.hcnkem.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xxk.chenzaomai.com

[R56] 远程拷贝
来源：http://xay.pycfn.com

scp file user@host:/path/
来源：http://rql.vehdjk.com

[R57] 远程执行命令
来源：http://olm.fktsv.cn

ssh user@host 'uptime'
来源：http://jwr.wangshuangyany.cn

[R58] 下载文件
来源：http://bxg.dianchejie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hmw.zhongyouzk.top

[R59] 发 POST JSON
来源：http://fqr.zdbjq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wuq.chenzaomai.com

[R60] 只看 HTTP 状态码
来源：http://nyg.mhx1999.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nxa.ybcxt.top

[R61] 磁盘占用
来源：http://neo.yongpay.top

df -h;  du -sh *
来源：http://dtu.wangshuangyany.cn

[R62] 找最占空间的文件
来源：http://ayi.hysaishi.cn

du -ah . | sort -rh | head -10
来源：http://kqo.pycfn.com

[R63] 内存与进程
来源：http://sqy.pengpengdd.cyou

free -h;  ps aux | grep nginx
来源：http://zva.yonumen.top

[R64] 结束进程
来源：http://fnm.sysykeji.top

kill -9 $(pgrep -f app.py)
来源：http://yyx.dashuyun.cn

[R65] 查看端口占用
来源：http://xov.52xcode.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vfv.hysaishi.cn

[R66] 定时任务
来源：http://dxb.nwbrower.top

crontab -e;  crontab -l
来源：http://yec.uphjek.com

[R67] 生成随机十六进制串
来源：http://hxr.vqdsnc.cn

openssl rand -hex 16
来源：http://jvz.hnxiangtu.top

[R68] 计算文件校验值
来源：http://amf.haohaochexian.top

sha256sum a.txt;  md5sum a.txt
来源：http://lke.hfpthk.cn

[R69] 生成随机密码
来源：http://dkw.gotoacloud.top

head -c 16 /dev/urandom | base64
来源：http://oil.ybcxt.top

[R70] 时间戳与互转
来源：http://lrt.smart0.xyz

date +%s;  date -d @1700000000
来源：http://rir.aibaodan.cn

[R71] 日期格式化
来源：http://pst.daxiang520.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wzr.yj20258888.top

[R72] 等待端口就绪
来源：http://mpz.hfpthk.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ted.quarkkingdee.top

[R73] 分割大日志
来源：http://hrv.meibo888.top

split -l 1000 big.log part_
来源：http://pzi.zycfv.cn

[R74] 批量重命名
来源：http://uft.fehbvm.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nuk.yanxiufei.cn

[R75] 导出环境变量
来源：http://ucn.dashuyun.cn

export PATH="$HOME/bin:$PATH"
来源：http://pky.fehbvm.com

[R76] 使用临时文件
来源：http://szr.vqdsnc.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tbt.hammf.cn

[R77] 读取用户输入
来源：http://ysb.shzxlz.cn

read -rp "请输入: " ans
来源：http://xtz.fktsv.cn

[R78] 交互式菜单
来源：http://hvz.chenzaomai.com

select opt in a b c; do echo "$opt"; break; done
来源：http://lim.epnwcf.com

[R79] 解析命令行选项
来源：http://ubq.svipenyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uwk.hywenlv.cn

[R80] 查看脚本执行耗时
来源：http://atn.jinqigufen.top

time ./run.sh
来源：http://emu.yj20258.top

================================================================================
来源：http://ndt.xuanzx.com

S. C / C++ 专题
来源：http://lvl.shuidangran.top

================================================================================
来源：http://upw.52xcode.cn

[S01] C：Hello World
来源：http://enu.nanxinkj.top

#include <stdio.h>
来源：http://ayg.haohaochexian.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://hoz.wangdashe.top

[S02] C：变量与格式化输出
来源：http://ydk.chenlongwang.top

int a = 10; printf("%d\n", a);
来源：http://ify.hfpthk.cn

[S03] C：读入整数
来源：http://ltd.nanxuanxn.top

int x; scanf("%d", &x);
来源：http://lba.fehbvm.com

[S04] C：字符串复制
来源：http://rit.yongpay.top

char dst[32]; strcpy(dst, "hi");
来源：http://tae.yj20258888.top

[S05] C：字符串长度
来源：http://cdb.aizwys.cn

strlen(s)
来源：http://cty.meibo888.top

[S06] C：字符串比较
来源：http://dcn.cashguo.top

strcmp(a, b) == 0
来源：http://vim.redwolf501.top

[S07] C：数组遍历求和
来源：http://qvu.zhaomingkeji.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dxj.jinghuilouyu.cn

[S08] C：动态内存分配与释放
来源：http://ejv.chenzaomai.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zal.aibaodan.cn

[S09] C：结构体定义与初始化
来源：http://tjz.kuanghao11.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://trn.fengsongda.top

[S10] C：指针与解引用
来源：http://wbc.daria6918.cn

int *p = &a;  *p = 5;
来源：http://kgy.zhiwuduotai.top

[S11] C：逐行读文件
来源：http://zit.pengpengdd.cyou


<!-- 参考信息 -->