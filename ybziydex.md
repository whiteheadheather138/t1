代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://mcg.feifeiyinyue.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jxq.ehwqpu.com

[Q43] 标量子查询
来源：http://chr.ybcxt.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mxi.quarkkingdee.top

[Q44] IN 子查询
来源：http://cii.hesvh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hzm.nanxinkj.top

[Q45] EXISTS 判断存在
来源：http://ffb.smart0.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wix.pengpengdd.cyou

[Q46] NOT EXISTS 判断不存在
来源：http://wzo.hnqzz.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ovx.vehdjk.com

[Q47] 与平均值比较
来源：http://nqx.fengsongda.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yks.zhaomingkeji.xyz

[Q48] CTE 公用表表达式
来源：http://iul.sxryk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cpm.ybcxt.top

SELECT * FROM t WHERE c > 5;
来源：http://pvr.dianchejie.cn

[Q49] 更新单行
来源：http://whk.jinqigufen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rlg.zdbjq.cn

[Q50] 批量更新
来源：http://jjk.ivvv.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nnq.zhijiandao.cn

[Q51] 用子查询更新
来源：http://bhk.xylfe.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gmb.yj20258.top

[Q52] 删除指定行
来源：http://tlm.cqqwz.cn

DELETE FROM users WHERE id = 10;
来源：http://dvv.yonumen.top

[Q53] 按条件删除
来源：http://biv.shzxlz.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://llb.ybcxt.top

[Q54] 清空表
来源：http://ltx.fzhhl.top

TRUNCATE TABLE logs;
来源：http://vbd.yangfankeji.com

[Q55] 排名（并列占位）
来源：http://fhu.hywenlv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ubv.9152youxi.cn

[Q56] 密集排名（并列不占位）
来源：http://gak.yanxiufei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vkk.yj20258888.top

[Q57] 行号
来源：http://mwr.316326.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rvo.hnqzz.top

[Q58] 累计求和
来源：http://jfc.jlsjyb.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://npr.tianlin.xyz

[Q59] 分组内累计
来源：http://hgq.dashuyun.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dix.andypj.xyz

[Q60] 取上一行 / 下一行
来源：http://abd.316326.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://twv.cucudq.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ony.uphjek.com

[Q61] 移动平均
来源：http://dym.daxiang520.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kvq.pycfn.com

[Q62] 分组占比
来源：http://lvv.yj20258.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jqs.zdbjq.cn

[Q63] 开启事务
来源：http://ily.shuidangran.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gci.cdnleiting.top

[Q64] 提交事务
来源：http://ffr.zhiwuduotai.top

COMMIT;
来源：http://cuu.nanxuanxn.top

[Q65] 回滚事务
来源：http://luh.jinqigufen.top

ROLLBACK;
来源：http://rvm.cucudq.cn

[Q66] 行锁查询
来源：http://sbp.hnqzz.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yra.guannengcc.top

[Q67] 设置隔离级别
来源：http://okr.xuetiantiany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vns.zhaomingkeji.xyz

[Q68] 保存点
来源：http://bcg.ppjwa.cn

SAVEPOINT sp1;
来源：http://kka.gaohongyu789.top

ROLLBACK TO sp1;
来源：http://wys.hysaishi.cn

[Q69] 查看执行计划
来源：http://otn.hammf.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bcq.ydjk.org.cn

[Q70] 更新统计信息
来源：http://hym.jinqigfzy.top

ANALYZE TABLE users;
来源：http://hiz.shanyushiyangtech.top

[Q71] 查看建表语句
来源：http://pzn.redwolf501.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bsa.c1oappe.top

[Q72] 查看索引
来源：http://qxo.ybcxt.top

SHOW INDEX FROM users;
来源：http://gdu.52xcode.cn

[Q73] 查看表状态
来源：http://hcn.yuxming.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://azs.kuanghao11.cn

[Q74] 强制使用索引
来源：http://uvi.hammf.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nff.jianghu66.top

[Q75] 日期格式化
来源：http://mko.xuanzx.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vlg.jinqigfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://say.nwbrower.top

[Q76] 按天统计
来源：http://iis.kuanghao11.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uth.ybcxt.top

[Q77] 时间加减
来源：http://fgb.feifeiyinyue.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://esf.shanyushiyangkeji.top

[Q78] 当前时间
来源：http://wll.zhijiandao.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://njb.dianchejie.cn

[Q79] 字符串拼接
来源：http://yyp.ydzc1.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lhn.zhijiandao.cn

[Q80] 字符串截取
来源：http://ekk.vehdjk.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pwi.shanyushiyangtech.top

[Q81] 字符串替换
来源：http://sbr.dashuyun.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mys.tian-w.cn

[Q82] 字符长度与字节长度
来源：http://aef.nanxinkj.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://epe.ydzc1.top

[Q83] 大小写转换
来源：http://two.ydzc1.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bud.tian-w.cn

[Q84] 去除首尾空格
来源：http://vil.jyoumei.cn

SELECT TRIM(name) FROM users;
来源：http://atv.gotoacloud.top

[Q85] 数值取整
来源：http://erd.yongpay.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://puq.redwolf501.top

[Q86] 读取 JSON 字段
来源：http://dvp.redwolf501.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://esn.zdqjudy.top

[Q87] JSON 字段做条件
来源：http://bac.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fbu.yj20258888.top

[Q88] 行转列（条件聚合）
来源：http://bky.snrcjt.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://efg.yj202588.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kuw.epnwcf.com

[Q89] 判断表是否存在
来源：http://pxy.jyoumei.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://daj.mhx1999.top

[Q90] 生成序号列
来源：http://edg.sysykeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gys.uphjek.com

================================================================================
来源：http://tke.yonumen.top

R. Bash 专题
来源：http://woq.uphjek.com

================================================================================
来源：http://vgl.cqqwz.cn

[R01] shebang 与严格模式
来源：http://qek.havefunace.top

#!/usr/bin/env bash
来源：http://age.pycfn.com

set -euo pipefail
来源：http://hld.xylfe.cn

[R02] 变量赋值与使用
来源：http://grm.epnwcf.com

name="Tom"; echo "$name"
来源：http://afz.hammf.cn

[R03] 只读变量
来源：http://nsp.epnwcf.com

readonly PI=3.14
来源：http://odz.zdbjq.cn

[R04] 位置参数
来源：http://xlh.andypj.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pvb.yj202588.top

[R05] 参数默认值
来源：http://jex.vqdsnc.cn

name="${1:-default}"
来源：http://gzs.zhongyouzk.top

[R06] 判断命令是否存在
来源：http://wff.yongpay.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fin.fzhhl.top

[R07] if 判断文件
来源：http://vmv.gogol.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ruy.jiagoushi.top

[R08] 数值比较
来源：http://vhd.gogol.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://exh.xinyue.icu

[R09] 字符串比较
来源：http://ase.havefunace.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ket.hysaishi.cn

[R10] 正则匹配
来源：http://gdc.zhijiandao.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wec.sxryk.cn

[R11] case 多分支
来源：http://zjn.yvedp.cn

case "$1" in
来源：http://sox.dashuyun.cn

start) echo "启动" ;;
来源：http://jcl.hongshengwenyu.top

stop)  echo "停止" ;;
来源：http://vgr.jianghu66.top

*)     echo "未知命令" ;;
来源：http://lun.zdqjudy.top

esac
来源：http://bmv.aibaodan.cn

[R12] for 遍历文件
来源：http://mux.zhixingplan.top

for f in *.txt; do echo "$f"; done
来源：http://mwo.jiagoushi.top

[R13] for 计数循环
来源：http://rqx.yanxiufei.cn

for i in {1..10}; do echo "$i"; done
来源：http://flf.zhaomingkeji.xyz

[R14] C 风格 for
来源：http://pmx.andypj.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rdm.ybcxt.top

[R15] while 逐行读文件
来源：http://yat.jqgfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rpv.epnwcf.com

[R16] until 等待条件
来源：http://has.aizwys.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qjd.bjfxy.top

[R17] 数组定义与取值
来源：http://dia.dashuyun.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gek.guannengcc.top

[R18] 遍历数组
来源：http://sww.dianchejie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qin.fehbvm.com

[R19] 数组长度
来源：http://uxv.hfpthk.cn

echo "${#arr[@]}"
来源：http://ufm.cheryme.top

[R20] 关联数组（字典）
来源：http://cqn.nanxuanxn.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ewq.jinghuilouyu.cn

[R21] 字符串长度
来源：http://ldj.tianlin.xyz

echo "${#s}"
来源：http://yor.meibo888.top

[R22] 截取子串
来源：http://oiv.zhengqikj.top

echo "${s:0:5}"
来源：http://dzy.epnwcf.com

[R23] 字符串替换
来源：http://luw.iojbl.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iix.kuanghao11.cn

[R24] 大小写转换
来源：http://oqn.fehbvm.com

echo "${s^^}"; echo "${s,,}"
来源：http://ldw.redwolf501.top

[R25] 去后缀 / 去前缀
来源：http://qkb.gotoacloud.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dxl.jlsjyb.cn

[R26] 命令替换
来源：http://yzm.haohaochexian.top

now=$(date +%F); echo "$now"
来源：http://kkj.chenzaomai.com

[R27] 算术展开
来源：http://smm.wangdashe.top

echo $((1 + 2 * 3))
来源：http://qmg.nwbrower.top

[R28] 浮点运算
来源：http://jcd.zhaomingkeji.xyz

echo "scale=2; 10/3" | bc
来源：http://wrv.smart0.xyz

[R29] 定义函数
来源：http://blv.ehwqpu.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wvy.zhoulong.xyz

[R30] 函数返回状态码
来源：http://oyr.bjfxy.top

f() { return 0; }; f || echo "失败了"
来源：http://qok.andypj.xyz

[R31] 局部变量
来源：http://gdg.cdnleiting.top

f() { local x=1; echo "$x"; }
来源：http://byy.ppjwa.cn

[R32] 参数个数校验
来源：http://bmx.daxiang520.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://aym.zhaomingkeji.xyz

[R33] 捕获错误并提示行号
来源：http://wwy.yanxiufei.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bmm.zycfv.cn

[R34] 退出时清理
来源：http://wsh.jlsjyb.cn

trap 'rm -f "$tmp"' EXIT
来源：http://efw.chenjidiqi.icu

[R35] 后台执行并等待
来源：http://vgj.yfazqb.com

sleep 5 & pid=$!; wait "$pid"
来源：http://cim.chenjidiqi.icu

[R36] 并发执行多个任务
来源：http://jlx.sweek.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hlg.yangfankeji.com

[R37] 把输出赋给变量
来源：http://fcy.shangyingyoupin.top

files=$(ls -1)
来源：http://lgq.fengsongda.top

[R38] 管道串联
来源：http://bsz.snrcjt.cn

cat a.txt | grep -i error | wc -l
来源：http://auw.bjfxy.top

[R39] 重定向标准输出与错误
来源：http://rwz.gogol.net.cn

cmd > out.log 2>&1
来源：http://gsk.nanxuanxn.top

[R40] 追加写日志
来源：http://zic.zhoulong.xyz

echo "log" >> out.log
来源：http://pwh.xingfuxueyuan.xyz

[R41] 丢弃输出
来源：http://koj.cdnleiting.top

cmd >/dev/null 2>&1
来源：http://xav.yj20258888.top

[R42] 输入重定向
来源：http://mux.jinyuanbaomall.cn

wc -l < a.txt
来源：http://uth.fzhhl.top

[R43] 按名字查找文件
来源：http://ili.jlsjyb.cn

find . -name "*.log" -type f
来源：http://ufv.vehdjk.com

[R44] 按修改时间查找
来源：http://bdo.xylfe.cn

find . -mtime -7 -type f
来源：http://gap.jqgfzy.top

[R45] 批量删除
来源：http://idy.yuanzhike.top

find . -name "*.tmp" -delete
来源：http://djo.hnqzz.top

[R46] 递归替换文件内容
来源：http://mmp.zhengqikj.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lvt.zdqjudy.top

[R47] sed 单行替换
来源：http://gch.iojbl.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sul.jinghuilouyu.cn

[R48] awk 取指定列
来源：http://bue.tanke756.top

awk '{print $1, $3}' a.txt
来源：http://krb.yangfankeji.com

[R49] awk 带条件
来源：http://tqx.cdnleiting.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nei.hnxiangtu.top

[R50] awk 求和
来源：http://ehc.jinghuilouyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://flk.quarkkingdee.top

[R51] 排序去重取前几
来源：http://gli.yfazqb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://pob.chenzaomai.com

[R52] 统计行数
来源：http://lvw.yuxming.cn

wc -l a.txt
来源：http://yxv.xinyue.icu

[R53] 查看文件头与实时尾
来源：http://fuu.hesvh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xgl.gogol.net.cn

[R54] 比较两个文件
来源：http://mib.aibaodan.cn

diff a.txt b.txt
来源：http://vcx.vehdjk.com

[R55] 压缩与解压
来源：http://jov.jyoumei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dlr.xziqi.cn

[R56] 远程拷贝
来源：http://bmg.sysykeji.top

scp file user@host:/path/
来源：http://xgu.hysaishi.cn

[R57] 远程执行命令
来源：http://pmg.jinqigufen.top

ssh user@host 'uptime'
来源：http://bqk.xziqi.cn

[R58] 下载文件
来源：http://brw.hongshengwenyu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wms.jyoumei.cn

[R59] 发 POST JSON
来源：http://alp.yongpay.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tsj.sufxvd.cn

[R60] 只看 HTTP 状态码
来源：http://wsx.yj20258.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fgu.wangdashe.top

[R61] 磁盘占用
来源：http://eee.xuanzx.com

df -h;  du -sh *
来源：http://tvv.shzxlz.cn

[R62] 找最占空间的文件
来源：http://qcb.zhoulong.xyz

du -ah . | sort -rh | head -10
来源：http://ngd.shangyingyoupin.top

[R63] 内存与进程
来源：http://gyj.zhaomingkeji.xyz

free -h;  ps aux | grep nginx
来源：http://uma.shuidangran.top

[R64] 结束进程
来源：http://gxb.ybcxt.top

kill -9 $(pgrep -f app.py)
来源：http://mjx.zhongyouzk.top

[R65] 查看端口占用
来源：http://obl.cqqwz.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dcu.zhaomingkeji.xyz

[R66] 定时任务
来源：http://oih.xuanzx.com

crontab -e;  crontab -l
来源：http://kmx.chenlongwang.top

[R67] 生成随机十六进制串
来源：http://gfn.xinyue.icu

openssl rand -hex 16
来源：http://vep.tian-w.cn

[R68] 计算文件校验值
来源：http://aib.jyoumei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://czl.ppjwa.cn

[R69] 生成随机密码
来源：http://gly.hongshengwenyu.top

head -c 16 /dev/urandom | base64
来源：http://fqm.yanxiufei.cn

[R70] 时间戳与互转
来源：http://ocx.hywenlv.cn

date +%s;  date -d @1700000000
来源：http://eug.fktsv.cn

[R71] 日期格式化
来源：http://ubr.jinqigfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kpi.jqgfzy.top

[R72] 等待端口就绪
来源：http://vkq.yuanzhike.top

until nc -z localhost 3306; do sleep 1; done
来源：http://gdw.andypj.xyz

[R73] 分割大日志
来源：http://ufk.aibaodan.cn

split -l 1000 big.log part_
来源：http://lfw.zhaomingkeji.xyz

[R74] 批量重命名
来源：http://bnb.zdbjq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uxf.guannengcc.top

[R75] 导出环境变量
来源：http://ona.birdmap.top

export PATH="$HOME/bin:$PATH"
来源：http://yxy.zhijiandao.cn

[R76] 使用临时文件
来源：http://fib.daria6918.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wvi.yj20258.top

[R77] 读取用户输入
来源：http://mpw.yonumen.top

read -rp "请输入: " ans
来源：http://zoy.xingfuxueyuan.xyz

[R78] 交互式菜单
来源：http://mwr.fktsv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sgn.c1oappe.top

[R79] 解析命令行选项
来源：http://yeb.yj20258888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gux.ywan-chungtsiang.top

[R80] 查看脚本执行耗时
来源：http://bgi.zhoulong.xyz

time ./run.sh
来源：http://ejg.haohaochexian.top

================================================================================
来源：http://ewl.yongpay.top

S. C / C++ 专题
来源：http://zcw.yuxming.cn

================================================================================
来源：http://kbc.shanyushiyangtech.top

[S01] C：Hello World
来源：http://osh.hfpthk.cn

#include <stdio.h>
来源：http://unw.wangdashe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wqw.hnqzz.top

[S02] C：变量与格式化输出
来源：http://cvm.jqgfzy.top

int a = 10; printf("%d\n", a);
来源：http://cqy.ehwqpu.com

[S03] C：读入整数
来源：http://mcq.wangdashe.top

int x; scanf("%d", &x);
来源：http://srs.cashguo.top

[S04] C：字符串复制
来源：http://qqx.xinyue.icu

char dst[32]; strcpy(dst, "hi");
来源：http://auu.zdbjq.cn

[S05] C：字符串长度
来源：http://pyr.zdqjudy.top

strlen(s)
来源：http://xsv.ywan-chungtsiang.top

[S06] C：字符串比较
来源：http://xxq.vqdsnc.cn

strcmp(a, b) == 0
来源：http://guu.jinqigfzy.top

[S07] C：数组遍历求和
来源：http://nlo.andypj.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kcb.jinghuilouyu.cn

[S08] C：动态内存分配与释放
来源：http://uoo.xuetiantiany.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qdh.cdnleiting.top

[S09] C：结构体定义与初始化
来源：http://jay.fengsongda.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ltp.xziqi.cn

[S10] C：指针与解引用
来源：http://ecp.quarkkingdee.top

int *p = &a;  *p = 5;
来源：http://fsz.pycfn.com

[S11] C：逐行读文件
来源：http://doc.sxryk.cn

FILE *f = fopen("a.txt", "r");
来源：http://xxp.hfpthk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dig.shangyingyoupin.top

fclose(f);
来源：http://nrs.zhiwuduotai.top

[S12] C：写文件
来源：http://pjk.chenjidiqi.icu


<!-- 参考信息 -->