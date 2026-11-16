代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://hju.sysykeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ruf.hcnkem.com

[Q43] 标量子查询
来源：http://rgu.c1oappe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mvb.guannengcc.top

[Q44] IN 子查询
来源：http://imi.zhiwuduotai.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kea.hysaishi.cn

[Q45] EXISTS 判断存在
来源：http://gwj.zdbjq.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ttv.shanyushiyangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://wun.ctjpmb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://twj.guannengcc.top

[Q47] 与平均值比较
来源：http://ovx.jqgufenzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ska.jinqigufen.top

[Q48] CTE 公用表表达式
来源：http://wyc.jinqigfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dhk.hfpthk.cn

SELECT * FROM t WHERE c > 5;
来源：http://tzm.ydjk.org.cn

[Q49] 更新单行
来源：http://arv.redwolf501.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cim.jiagoushi.top

[Q50] 批量更新
来源：http://jym.yuanzhike.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vov.fengsongda.top

[Q51] 用子查询更新
来源：http://cwq.birdmap.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vnz.aibaodan.cn

[Q52] 删除指定行
来源：http://lik.wangshuangyany.cn

DELETE FROM users WHERE id = 10;
来源：http://xop.aizwys.cn

[Q53] 按条件删除
来源：http://jha.sysykeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://spu.quarkkingdee.top

[Q54] 清空表
来源：http://npd.zhongyouzk.top

TRUNCATE TABLE logs;
来源：http://fas.9152youxi.cn

[Q55] 排名（并列占位）
来源：http://gsu.mhx1999.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://phg.tarul.cn

[Q56] 密集排名（并列不占位）
来源：http://rbu.fanxiaobao.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wtt.aibaodan.cn

[Q57] 行号
来源：http://ikc.shanyushiyangtech.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://udh.cdnleiting.top

[Q58] 累计求和
来源：http://giw.dashuyun.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nly.yueranfly.top

[Q59] 分组内累计
来源：http://zor.aizwys.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vop.xuanzx.com

[Q60] 取上一行 / 下一行
来源：http://kxm.gogol.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://evr.zhongyouzk.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://oqi.feifeiyinyue.top

[Q61] 移动平均
来源：http://tey.jiagoushi.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zec.gotoacloud.top

[Q62] 分组占比
来源：http://ahx.yvedp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kjz.fzhhl.top

[Q63] 开启事务
来源：http://eno.havefunace.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rkp.yuanzhike.top

[Q64] 提交事务
来源：http://wmg.andypj.xyz

COMMIT;
来源：http://ell.sufxvd.cn

[Q65] 回滚事务
来源：http://yot.jlsjyb.cn

ROLLBACK;
来源：http://gqq.xingfuxueyuan.xyz

[Q66] 行锁查询
来源：http://mbv.daria6918.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nvc.cucudq.cn

[Q67] 设置隔离级别
来源：http://wky.fktsv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tph.zhengqikj.top

[Q68] 保存点
来源：http://yay.pengpengdd.cyou

SAVEPOINT sp1;
来源：http://hvd.52xcode.cn

ROLLBACK TO sp1;
来源：http://ogr.ybcxt.top

[Q69] 查看执行计划
来源：http://kxq.chenzaomai.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://orw.yueranfly.top

[Q70] 更新统计信息
来源：http://tzh.mhx1999.top

ANALYZE TABLE users;
来源：http://lsw.9152youxi.cn

[Q71] 查看建表语句
来源：http://zdg.shanyushiyangtech.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vfh.feifeiyinyue.top

[Q72] 查看索引
来源：http://lkt.yvedp.cn

SHOW INDEX FROM users;
来源：http://ulf.yanxiufei.cn

[Q73] 查看表状态
来源：http://lbd.yj20258888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vmm.sjlbkw.cn

[Q74] 强制使用索引
来源：http://rql.c1oappe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zfb.shzxlz.cn

[Q75] 日期格式化
来源：http://lyj.meibo888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nql.fanxiaobao.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yjj.ehwqpu.com

[Q76] 按天统计
来源：http://dcj.daria6918.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ilk.shzxlz.cn

[Q77] 时间加减
来源：http://exw.xuetiantiany.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qkj.zhaomingkeji.xyz

[Q78] 当前时间
来源：http://ghv.hnqzz.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mkh.ydzc1.top

[Q79] 字符串拼接
来源：http://zeu.havefunace.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://enb.gogol.net.cn

[Q80] 字符串截取
来源：http://ajy.wangdashe.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cfo.fktsv.cn

[Q81] 字符串替换
来源：http://byx.yanxiufei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://alj.nanxinkj.top

[Q82] 字符长度与字节长度
来源：http://mmg.316326.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sus.chenjidiqi.icu

[Q83] 大小写转换
来源：http://oda.iojbl.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://elz.yueranfly.top

[Q84] 去除首尾空格
来源：http://vrs.chenlongwang.top

SELECT TRIM(name) FROM users;
来源：http://jpy.birdmap.top

[Q85] 数值取整
来源：http://zjs.smart0.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tgh.fzhhl.top

[Q86] 读取 JSON 字段
来源：http://fmv.guowangkeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://omn.dashuyun.cn

[Q87] JSON 字段做条件
来源：http://fxr.yj202588.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ava.zhaomingkeji.xyz

[Q88] 行转列（条件聚合）
来源：http://cjm.ydjk.org.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ooo.cqqwz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ugr.xingfuxueyuan.xyz

[Q89] 判断表是否存在
来源：http://lyo.pycfn.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vwv.ppjwa.cn

[Q90] 生成序号列
来源：http://vzd.jianghu66.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://okb.hammf.cn

================================================================================
来源：http://fqu.hysaishi.cn

R. Bash 专题
来源：http://yyw.vqdsnc.cn

================================================================================
来源：http://dfx.jqgfzy.top

[R01] shebang 与严格模式
来源：http://oyr.shanyushiyangtech.top

#!/usr/bin/env bash
来源：http://rlo.zycfv.cn

set -euo pipefail
来源：http://yml.cashguo.top

[R02] 变量赋值与使用
来源：http://jce.birdmap.top

name="Tom"; echo "$name"
来源：http://inm.gotoacloud.top

[R03] 只读变量
来源：http://igt.hongshengwenyu.top

readonly PI=3.14
来源：http://uef.svipenyu.cn

[R04] 位置参数
来源：http://yga.jinqigufen.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nef.jianghu66.top

[R05] 参数默认值
来源：http://ehe.shanyushiyangkeji.top

name="${1:-default}"
来源：http://spn.hcnkem.com

[R06] 判断命令是否存在
来源：http://vqt.ehwqpu.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pjt.daxiang520.top

[R07] if 判断文件
来源：http://kbs.fengsongda.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://opl.yj20258.top

[R08] 数值比较
来源：http://qxl.shuidangran.top

if (( a > b )); then echo "a 更大"; fi
来源：http://yrj.zhoulong.xyz

[R09] 字符串比较
来源：http://qfb.yuxming.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ttb.guannengcc.top

[R10] 正则匹配
来源：http://vkr.ppjwa.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://req.guowangkeji.top

[R11] case 多分支
来源：http://uys.gaohongyu789.top

case "$1" in
来源：http://wph.jinghuilouyu.cn

start) echo "启动" ;;
来源：http://wmm.birdmap.top

stop)  echo "停止" ;;
来源：http://ybo.guannengcc.top

*)     echo "未知命令" ;;
来源：http://zge.jianghu66.top

esac
来源：http://kty.birdmap.top

[R12] for 遍历文件
来源：http://mae.kuanghao11.cn

for f in *.txt; do echo "$f"; done
来源：http://lkx.yj20258.top

[R13] for 计数循环
来源：http://znw.gaohongyu789.top

for i in {1..10}; do echo "$i"; done
来源：http://fcv.ivvv.top

[R14] C 风格 for
来源：http://tfl.svipenyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zxq.snrcjt.cn

[R15] while 逐行读文件
来源：http://mcg.ctjpmb.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zbf.yfazqb.com

[R16] until 等待条件
来源：http://xwb.zdqjudy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wbq.xylfe.cn

[R17] 数组定义与取值
来源：http://hqx.havefunace.top

arr=(a b c); echo "${arr[0]}"
来源：http://ojc.yanxiufei.cn

[R18] 遍历数组
来源：http://dqa.cucudq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nrf.c1oappe.top

[R19] 数组长度
来源：http://tny.kuanghao11.cn

echo "${#arr[@]}"
来源：http://aeb.jianghu66.top

[R20] 关联数组（字典）
来源：http://swp.yuxming.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nlg.gotoacloud.top

[R21] 字符串长度
来源：http://atv.andypj.xyz

echo "${#s}"
来源：http://jin.ivvv.top

[R22] 截取子串
来源：http://cvs.ywan-chungtsiang.top

echo "${s:0:5}"
来源：http://fej.yj202588.top

[R23] 字符串替换
来源：http://zyd.zhijiandao.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qfr.nanxuanxn.top

[R24] 大小写转换
来源：http://hsa.cucudq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ubm.yonumen.top

[R25] 去后缀 / 去前缀
来源：http://bom.ppjwa.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nzs.jiagoushi.top

[R26] 命令替换
来源：http://cka.0kj1m.cn

now=$(date +%F); echo "$now"
来源：http://mmq.jlsjyb.cn

[R27] 算术展开
来源：http://lfj.hammf.cn

echo $((1 + 2 * 3))
来源：http://cqq.hnqzz.top

[R28] 浮点运算
来源：http://tpa.jinqigufen.top

echo "scale=2; 10/3" | bc
来源：http://den.aibaodan.cn

[R29] 定义函数
来源：http://tpc.uphjek.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nqe.yuxming.cn

[R30] 函数返回状态码
来源：http://pbk.316326.xyz

f() { return 0; }; f || echo "失败了"
来源：http://hoa.yj20258.top

[R31] 局部变量
来源：http://pwq.wangdashe.top

f() { local x=1; echo "$x"; }
来源：http://dvc.andypj.xyz

[R32] 参数个数校验
来源：http://hbm.bjfxy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vkt.shanyushiyangtech.top

[R33] 捕获错误并提示行号
来源：http://sxv.wangshuangyany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mao.quarkkingdee.top

[R34] 退出时清理
来源：http://cqf.ydjk.org.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hiu.gzhubu.top

[R35] 后台执行并等待
来源：http://kpj.xingfuxueyuan.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://odi.hnxiangtu.top

[R36] 并发执行多个任务
来源：http://wfj.yonumen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hjf.nwbrower.top

[R37] 把输出赋给变量
来源：http://dgr.pycfn.com

files=$(ls -1)
来源：http://uzc.zhijiandao.cn

[R38] 管道串联
来源：http://mco.316326.xyz

cat a.txt | grep -i error | wc -l
来源：http://nbr.yj20258888.top

[R39] 重定向标准输出与错误
来源：http://gry.zhixingplan.top

cmd > out.log 2>&1
来源：http://qrt.hongshengwenyu.top

[R40] 追加写日志
来源：http://gxa.zhijiandao.cn

echo "log" >> out.log
来源：http://trc.yfazqb.com

[R41] 丢弃输出
来源：http://fva.nwbrower.top

cmd >/dev/null 2>&1
来源：http://lgj.hesvh.cn

[R42] 输入重定向
来源：http://lbd.mhx1999.top

wc -l < a.txt
来源：http://alv.hnqzz.top

[R43] 按名字查找文件
来源：http://gen.zhijiandao.cn

find . -name "*.log" -type f
来源：http://auf.tarul.cn

[R44] 按修改时间查找
来源：http://zps.epnwcf.com

find . -mtime -7 -type f
来源：http://nnb.shanyushiyangkeji.top

[R45] 批量删除
来源：http://bci.cdnleiting.top

find . -name "*.tmp" -delete
来源：http://fey.bjfxy.top

[R46] 递归替换文件内容
来源：http://rkm.feifeiyinyue.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ptc.shangyingyoupin.top

[R47] sed 单行替换
来源：http://hth.hnqzz.top

sed -i 's/foo/bar/g' a.txt
来源：http://wrs.chenlongwang.top

[R48] awk 取指定列
来源：http://wxc.svipenyu.cn

awk '{print $1, $3}' a.txt
来源：http://urm.hywenlv.cn

[R49] awk 带条件
来源：http://kgi.hnxiangtu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zzw.yueranfly.top

[R50] awk 求和
来源：http://ahe.shzxlz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://phi.uphjek.com

[R51] 排序去重取前几
来源：http://wdu.chenlongwang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://sew.tanke756.top

[R52] 统计行数
来源：http://dek.xingfuxueyuan.xyz

wc -l a.txt
来源：http://jxm.zycfv.cn

[R53] 查看文件头与实时尾
来源：http://luk.0kj1m.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yjc.smart0.xyz

[R54] 比较两个文件
来源：http://wyj.yanxiufei.cn

diff a.txt b.txt
来源：http://kcc.jianghu66.top

[R55] 压缩与解压
来源：http://jer.guowangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mmi.shanyushiyangkeji.top

[R56] 远程拷贝
来源：http://jxh.hongshengwenyu.top

scp file user@host:/path/
来源：http://jlg.shanyushiyangkeji.top

[R57] 远程执行命令
来源：http://gfk.zhiwuduotai.top

ssh user@host 'uptime'
来源：http://nij.ydjk.org.cn

[R58] 下载文件
来源：http://alw.meibo888.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tyk.yuxming.cn

[R59] 发 POST JSON
来源：http://ujs.cucudq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gbb.xuetiantiany.cn

[R60] 只看 HTTP 状态码
来源：http://cpx.bjfxy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lgq.hammf.cn

[R61] 磁盘占用
来源：http://cxo.vqdsnc.cn

df -h;  du -sh *
来源：http://jwb.epnwcf.com

[R62] 找最占空间的文件
来源：http://okc.xinyue.icu

du -ah . | sort -rh | head -10
来源：http://mln.birdmap.top

[R63] 内存与进程
来源：http://fvu.birdmap.top

free -h;  ps aux | grep nginx
来源：http://eay.cdnleiting.top

[R64] 结束进程
来源：http://ihn.ywan-chungtsiang.top

kill -9 $(pgrep -f app.py)
来源：http://ixl.hysaishi.cn

[R65] 查看端口占用
来源：http://kcq.jyoumei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ftp.shanyushiyangtech.top

[R66] 定时任务
来源：http://kje.fanxiaobao.xyz

crontab -e;  crontab -l
来源：http://vzj.yuanzhike.top

[R67] 生成随机十六进制串
来源：http://xih.jqgufenzy.top

openssl rand -hex 16
来源：http://slj.fehbvm.com

[R68] 计算文件校验值
来源：http://xgr.fengsongda.top

sha256sum a.txt;  md5sum a.txt
来源：http://cti.xziqi.cn

[R69] 生成随机密码
来源：http://knr.hfpthk.cn

head -c 16 /dev/urandom | base64
来源：http://rxv.sxryk.cn

[R70] 时间戳与互转
来源：http://xpi.yvedp.cn

date +%s;  date -d @1700000000
来源：http://har.redwolf501.top

[R71] 日期格式化
来源：http://dct.jinqigufen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://yvc.gogol.net.cn

[R72] 等待端口就绪
来源：http://xnl.vehdjk.com

until nc -z localhost 3306; do sleep 1; done
来源：http://pbr.shangyingyoupin.top

[R73] 分割大日志
来源：http://vkh.ppjwa.cn

split -l 1000 big.log part_
来源：http://yhs.bbcook.cn

[R74] 批量重命名
来源：http://gwl.bjfxy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mfw.cqqwz.cn

[R75] 导出环境变量
来源：http://lig.fanxiaobao.xyz

export PATH="$HOME/bin:$PATH"
来源：http://mub.vqdsnc.cn

[R76] 使用临时文件
来源：http://mim.gogol.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nlw.xuanzx.com

[R77] 读取用户输入
来源：http://nfi.tian-w.cn

read -rp "请输入: " ans
来源：http://ikd.sxryk.cn

[R78] 交互式菜单
来源：http://bed.c1oappe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vxe.quarkkingdee.top

[R79] 解析命令行选项
来源：http://sdv.shanyushiyangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qgg.jqgufenzy.top

[R80] 查看脚本执行耗时
来源：http://fxw.yj20258888.top

time ./run.sh
来源：http://ztk.jinqigfzy.top

================================================================================
来源：http://jdc.shzxlz.cn

S. C / C++ 专题
来源：http://ksc.jlsjyb.cn

================================================================================
来源：http://bat.c1oappe.top

[S01] C：Hello World
来源：http://fsl.ywan-chungtsiang.top

#include <stdio.h>
来源：http://nti.yfazqb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://xbs.yvedp.cn

[S02] C：变量与格式化输出
来源：http://cio.jyoumei.cn

int a = 10; printf("%d\n", a);
来源：http://zdm.yanxiufei.cn

[S03] C：读入整数
来源：http://tfb.yangfankeji.com

int x; scanf("%d", &x);
来源：http://uah.jinqigufen.top

[S04] C：字符串复制
来源：http://ipp.wangshuangyany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ypi.yonumen.top

[S05] C：字符串长度
来源：http://wqg.sjlbkw.cn

strlen(s)
来源：http://frq.chenlongwang.top

[S06] C：字符串比较
来源：http://uhb.hongshengwenyu.top

strcmp(a, b) == 0
来源：http://zwp.aibaodan.cn

[S07] C：数组遍历求和
来源：http://wmd.zhongyouzk.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dog.yuxming.cn

[S08] C：动态内存分配与释放
来源：http://ddy.cqqwz.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ggl.jiagoushi.top

[S09] C：结构体定义与初始化
来源：http://aqy.sjlbkw.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gql.fktsv.cn

[S10] C：指针与解引用
来源：http://bmo.hammf.cn

int *p = &a;  *p = 5;
来源：http://haf.kuanghao11.cn

[S11] C：逐行读文件
来源：http://cpa.hnxiangtu.top

FILE *f = fopen("a.txt", "r");
来源：http://mdc.jinyuanbaomall.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://evf.yj20258.top

fclose(f);
来源：http://nap.ppjwa.cn

[S12] C：写文件
来源：http://vnn.jinyuanbaomall.cn


<!-- 参考信息 -->