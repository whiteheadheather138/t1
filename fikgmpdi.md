代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://fgc.bjfxy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hth.ivvv.top

[Q47] 与平均值比较
来源：http://efe.tarul.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mwk.smart0.xyz

[Q48] CTE 公用表表达式
来源：http://nxc.sxryk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nbh.gotoacloud.top

SELECT * FROM t WHERE c > 5;
来源：http://sbo.hysaishi.cn

[Q49] 更新单行
来源：http://bxt.xuetiantiany.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pxj.haohaochexian.top

[Q50] 批量更新
来源：http://xtp.zhixingplan.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uxi.jlsjyb.cn

[Q51] 用子查询更新
来源：http://jmh.ehwqpu.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zat.yj202588.top

[Q52] 删除指定行
来源：http://nze.zycfv.cn

DELETE FROM users WHERE id = 10;
来源：http://nja.fengsongda.top

[Q53] 按条件删除
来源：http://vus.jinqigufen.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dlq.zhijiandao.cn

[Q54] 清空表
来源：http://zbp.andypj.xyz

TRUNCATE TABLE logs;
来源：http://mvg.havefunace.top

[Q55] 排名（并列占位）
来源：http://dwq.xingfuxueyuan.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tya.iojbl.cn

[Q56] 密集排名（并列不占位）
来源：http://rhz.hysaishi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jqc.bjfxy.top

[Q57] 行号
来源：http://uml.xuanzx.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://iog.aizwys.cn

[Q58] 累计求和
来源：http://niv.zhoulong.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zgz.guannengcc.top

[Q59] 分组内累计
来源：http://ycc.uphjek.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qcm.gogol.net.cn

[Q60] 取上一行 / 下一行
来源：http://nrp.cucudq.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ypu.epnwcf.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zml.hesvh.cn

[Q61] 移动平均
来源：http://uzv.ydjk.org.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ubc.aibaodan.cn

[Q62] 分组占比
来源：http://bhg.sxryk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ptu.yangfankeji.com

[Q63] 开启事务
来源：http://tly.sjlbkw.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dmt.zycfv.cn

[Q64] 提交事务
来源：http://osb.hnxiangtu.top

COMMIT;
来源：http://avq.yj20258888.top

[Q65] 回滚事务
来源：http://wog.dianchejie.cn

ROLLBACK;
来源：http://olw.zhengqikj.top

[Q66] 行锁查询
来源：http://dqd.jqgufenzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mtq.jianghu66.top

[Q67] 设置隔离级别
来源：http://ldl.yanxiufei.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tmx.mhx1999.top

[Q68] 保存点
来源：http://njb.tanke756.top

SAVEPOINT sp1;
来源：http://feb.xingfuxueyuan.xyz

ROLLBACK TO sp1;
来源：http://chu.havefunace.top

[Q69] 查看执行计划
来源：http://ims.jinyuanbaomall.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ift.shanyushiyangkeji.top

[Q70] 更新统计信息
来源：http://kos.ehwqpu.com

ANALYZE TABLE users;
来源：http://rex.yj20258.top

[Q71] 查看建表语句
来源：http://pzm.cucudq.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ntr.jinyuanbaomall.cn

[Q72] 查看索引
来源：http://htg.chenjidiqi.icu

SHOW INDEX FROM users;
来源：http://hqr.jinqigufen.top

[Q73] 查看表状态
来源：http://qox.yj20258888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wft.0kj1m.cn

[Q74] 强制使用索引
来源：http://zhl.yj20258888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mux.316326.xyz

[Q75] 日期格式化
来源：http://uex.zhengqikj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vgv.ehwqpu.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jfo.aibaodan.cn

[Q76] 按天统计
来源：http://rjy.redwolf501.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://flo.havefunace.top

[Q77] 时间加减
来源：http://vnf.9152youxi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ibz.hysaishi.cn

[Q78] 当前时间
来源：http://shi.jinqigufen.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://iih.xingfuxueyuan.xyz

[Q79] 字符串拼接
来源：http://cpj.c1oappe.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xgu.jyoumei.cn

[Q80] 字符串截取
来源：http://ujc.andypj.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ocx.yfazqb.com

[Q81] 字符串替换
来源：http://zvo.yj20258888.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://orb.tian-w.cn

[Q82] 字符长度与字节长度
来源：http://bbg.daxiang520.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ntm.sweek.top

[Q83] 大小写转换
来源：http://vso.hammf.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yym.zycfv.cn

[Q84] 去除首尾空格
来源：http://imo.tianlin.xyz

SELECT TRIM(name) FROM users;
来源：http://mvm.andypj.xyz

[Q85] 数值取整
来源：http://xzj.hfpthk.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xsz.sysykeji.top

[Q86] 读取 JSON 字段
来源：http://fje.gogol.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uar.xuanzx.com

[Q87] JSON 字段做条件
来源：http://vwj.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yyx.hnqzz.top

[Q88] 行转列（条件聚合）
来源：http://rfe.aizwys.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://iqi.hfpthk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vqt.yfazqb.com

[Q89] 判断表是否存在
来源：http://ybf.chenzaomai.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vee.hnqzz.top

[Q90] 生成序号列
来源：http://rkk.cucudq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rio.gogol.net.cn

================================================================================
来源：http://qdn.jinyuanbaomall.cn

R. Bash 专题
来源：http://wfq.sysykeji.top

================================================================================
来源：http://mgk.jlsjyb.cn

[R01] shebang 与严格模式
来源：http://cej.snrcjt.cn

#!/usr/bin/env bash
来源：http://pda.0kj1m.cn

set -euo pipefail
来源：http://qje.xylfe.cn

[R02] 变量赋值与使用
来源：http://uuu.yuxming.cn

name="Tom"; echo "$name"
来源：http://adc.hywenlv.cn

[R03] 只读变量
来源：http://tif.cashguo.top

readonly PI=3.14
来源：http://set.nanxuanxn.top

[R04] 位置参数
来源：http://kwy.yueranfly.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kye.pengpengdd.cyou

[R05] 参数默认值
来源：http://fpl.9152youxi.cn

name="${1:-default}"
来源：http://cit.0kj1m.cn

[R06] 判断命令是否存在
来源：http://nlk.c1oappe.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://egx.ctjpmb.com

[R07] if 判断文件
来源：http://psa.fengsongda.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ren.xziqi.cn

[R08] 数值比较
来源：http://lgf.iojbl.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zbb.yfazqb.com

[R09] 字符串比较
来源：http://gni.hysaishi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mpp.chenlongwang.top

[R10] 正则匹配
来源：http://kax.guannengcc.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mym.yuanzhike.top

[R11] case 多分支
来源：http://skd.ybcxt.top

case "$1" in
来源：http://tct.zhengqikj.top

start) echo "启动" ;;
来源：http://nbo.tian-w.cn

stop)  echo "停止" ;;
来源：http://ajk.ydzc1.top

*)     echo "未知命令" ;;
来源：http://imt.fanxiaobao.xyz

esac
来源：http://kjp.guowangkeji.top

[R12] for 遍历文件
来源：http://rjf.fengsongda.top

for f in *.txt; do echo "$f"; done
来源：http://puq.zycfv.cn

[R13] for 计数循环
来源：http://lzh.vqdsnc.cn

for i in {1..10}; do echo "$i"; done
来源：http://uwz.chenjidiqi.icu

[R14] C 风格 for
来源：http://fcr.yangfankeji.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ilw.zhengqikj.top

[R15] while 逐行读文件
来源：http://jaz.jlsjyb.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rof.gotoacloud.top

[R16] until 等待条件
来源：http://ccc.shanyushiyangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hpv.jqgufenzy.top

[R17] 数组定义与取值
来源：http://gmv.316326.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://sqx.quarkkingdee.top

[R18] 遍历数组
来源：http://wzw.shanyushiyangtech.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wcv.chenlongwang.top

[R19] 数组长度
来源：http://drd.zhongyouzk.top

echo "${#arr[@]}"
来源：http://exs.quarkkingdee.top

[R20] 关联数组（字典）
来源：http://cre.smart0.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ygx.gotoacloud.top

[R21] 字符串长度
来源：http://ypd.yfazqb.com

echo "${#s}"
来源：http://mtx.yonumen.top

[R22] 截取子串
来源：http://mfd.iojbl.cn

echo "${s:0:5}"
来源：http://qmz.iojbl.cn

[R23] 字符串替换
来源：http://luj.pengpengdd.cyou

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vcj.sxryk.cn

[R24] 大小写转换
来源：http://kmo.bjfxy.top

echo "${s^^}"; echo "${s,,}"
来源：http://rrl.yj20258.top

[R25] 去后缀 / 去前缀
来源：http://xxn.zhijiandao.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gvd.fengsongda.top

[R26] 命令替换
来源：http://nao.guannengcc.top

now=$(date +%F); echo "$now"
来源：http://qck.xziqi.cn

[R27] 算术展开
来源：http://rvt.nwbrower.top

echo $((1 + 2 * 3))
来源：http://wil.andypj.xyz

[R28] 浮点运算
来源：http://knd.zycfv.cn

echo "scale=2; 10/3" | bc
来源：http://jpa.yvedp.cn

[R29] 定义函数
来源：http://yef.sweek.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://auk.cashguo.top

[R30] 函数返回状态码
来源：http://uks.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://qns.smart0.xyz

[R31] 局部变量
来源：http://njd.hammf.cn

f() { local x=1; echo "$x"; }
来源：http://wrl.zhiwuduotai.top

[R32] 参数个数校验
来源：http://mmi.gaohongyu789.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://stm.zhoulong.xyz

[R33] 捕获错误并提示行号
来源：http://lvi.andypj.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tid.ywan-chungtsiang.top

[R34] 退出时清理
来源：http://pyj.zhengqikj.top

trap 'rm -f "$tmp"' EXIT
来源：http://wfw.316326.xyz

[R35] 后台执行并等待
来源：http://jmk.sysykeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wkk.wangdashe.top

[R36] 并发执行多个任务
来源：http://ded.xuanzx.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cvt.jqgufenzy.top

[R37] 把输出赋给变量
来源：http://dwx.zdqjudy.top

files=$(ls -1)
来源：http://gda.fengsongda.top

[R38] 管道串联
来源：http://tin.ybcxt.top

cat a.txt | grep -i error | wc -l
来源：http://ixn.guowangkeji.top

[R39] 重定向标准输出与错误
来源：http://slb.xziqi.cn

cmd > out.log 2>&1
来源：http://utw.ppjwa.cn

[R40] 追加写日志
来源：http://wda.yueranfly.top

echo "log" >> out.log
来源：http://gff.xuanzx.com

[R41] 丢弃输出
来源：http://hsc.zhijiandao.cn

cmd >/dev/null 2>&1
来源：http://hyh.shzxlz.cn

[R42] 输入重定向
来源：http://yed.9152youxi.cn

wc -l < a.txt
来源：http://irb.xuetiantiany.cn

[R43] 按名字查找文件
来源：http://yfi.cheryme.top

find . -name "*.log" -type f
来源：http://pfp.52xcode.cn

[R44] 按修改时间查找
来源：http://oyc.birdmap.top

find . -mtime -7 -type f
来源：http://qev.hywenlv.cn

[R45] 批量删除
来源：http://qsl.hywenlv.cn

find . -name "*.tmp" -delete
来源：http://gzm.vqdsnc.cn

[R46] 递归替换文件内容
来源：http://ail.feifeiyinyue.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mwj.smart0.xyz

[R47] sed 单行替换
来源：http://ndz.cashguo.top

sed -i 's/foo/bar/g' a.txt
来源：http://fwp.svipenyu.cn

[R48] awk 取指定列
来源：http://ozj.fanxiaobao.xyz

awk '{print $1, $3}' a.txt
来源：http://pqf.wangdashe.top

[R49] awk 带条件
来源：http://kdb.ivvv.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sqg.zhoulong.xyz

[R50] awk 求和
来源：http://kni.yfazqb.com

awk '{s += $2} END {print s}' a.txt
来源：http://pth.fehbvm.com

[R51] 排序去重取前几
来源：http://qnu.hnxiangtu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ijy.smart0.xyz

[R52] 统计行数
来源：http://auh.andypj.xyz

wc -l a.txt
来源：http://qqg.shzxlz.cn

[R53] 查看文件头与实时尾
来源：http://gmj.jlsjyb.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nes.gogol.net.cn

[R54] 比较两个文件
来源：http://jiv.c1oappe.top

diff a.txt b.txt
来源：http://auu.9152youxi.cn

[R55] 压缩与解压
来源：http://tqv.yvedp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zmb.hysaishi.cn

[R56] 远程拷贝
来源：http://mez.wangshuangyany.cn

scp file user@host:/path/
来源：http://gfq.zhongyouzk.top

[R57] 远程执行命令
来源：http://kgu.tian-w.cn

ssh user@host 'uptime'
来源：http://okp.0kj1m.cn

[R58] 下载文件
来源：http://qjd.aizwys.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uei.ctjpmb.com

[R59] 发 POST JSON
来源：http://axa.52xcode.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://arg.birdmap.top

[R60] 只看 HTTP 状态码
来源：http://qdx.ywan-chungtsiang.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zfv.zhongyouzk.top

[R61] 磁盘占用
来源：http://gmm.guannengcc.top

df -h;  du -sh *
来源：http://dif.ctjpmb.com

[R62] 找最占空间的文件
来源：http://het.ehwqpu.com

du -ah . | sort -rh | head -10
来源：http://eym.yonumen.top

[R63] 内存与进程
来源：http://fih.ybcxt.top

free -h;  ps aux | grep nginx
来源：http://omm.ppjwa.cn

[R64] 结束进程
来源：http://yqn.nanxinkj.top

kill -9 $(pgrep -f app.py)
来源：http://kpn.cashguo.top

[R65] 查看端口占用
来源：http://uxq.redwolf501.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lis.52xcode.cn

[R66] 定时任务
来源：http://qlm.gotoacloud.top

crontab -e;  crontab -l
来源：http://bie.xinyue.icu

[R67] 生成随机十六进制串
来源：http://phy.zycfv.cn

openssl rand -hex 16
来源：http://czw.uphjek.com

[R68] 计算文件校验值
来源：http://aqk.fktsv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dyv.daria6918.cn

[R69] 生成随机密码
来源：http://jtm.daxiang520.top

head -c 16 /dev/urandom | base64
来源：http://rin.feifeiyinyue.top

[R70] 时间戳与互转
来源：http://sag.aibaodan.cn

date +%s;  date -d @1700000000
来源：http://xss.guannengcc.top

[R71] 日期格式化
来源：http://yer.cdnleiting.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zns.fehbvm.com

[R72] 等待端口就绪
来源：http://wjx.tarul.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lof.zycfv.cn

[R73] 分割大日志
来源：http://rrc.pycfn.com

split -l 1000 big.log part_
来源：http://jnq.vqdsnc.cn

[R74] 批量重命名
来源：http://mck.sweek.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yxh.hcnkem.com

[R75] 导出环境变量
来源：http://luj.hnqzz.top

export PATH="$HOME/bin:$PATH"
来源：http://kjo.bjfxy.top

[R76] 使用临时文件
来源：http://dgz.jianghu66.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vqc.zhongyouzk.top

[R77] 读取用户输入
来源：http://wnc.dianchejie.cn

read -rp "请输入: " ans
来源：http://ubj.ctjpmb.com

[R78] 交互式菜单
来源：http://rbn.yj20258.top

select opt in a b c; do echo "$opt"; break; done
来源：http://sjz.xinyue.icu

[R79] 解析命令行选项
来源：http://mgc.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hla.hammf.cn

[R80] 查看脚本执行耗时
来源：http://nno.hysaishi.cn

time ./run.sh
来源：http://xzq.xinyue.icu

================================================================================
来源：http://iqd.andypj.xyz

S. C / C++ 专题
来源：http://sbk.zhoulong.xyz

================================================================================
来源：http://apb.iojbl.cn

[S01] C：Hello World
来源：http://rqy.gzhubu.top

#include <stdio.h>
来源：http://yly.ctjpmb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://seu.tian-w.cn

[S02] C：变量与格式化输出
来源：http://cie.zhijiandao.cn

int a = 10; printf("%d\n", a);
来源：http://cma.ybcxt.top

[S03] C：读入整数
来源：http://auw.aibaodan.cn

int x; scanf("%d", &x);
来源：http://brl.nanxuanxn.top

[S04] C：字符串复制
来源：http://dsc.ivvv.top

char dst[32]; strcpy(dst, "hi");
来源：http://tkh.xuanzx.com

[S05] C：字符串长度
来源：http://fbg.aizwys.cn

strlen(s)
来源：http://tai.sjlbkw.cn

[S06] C：字符串比较
来源：http://jrl.jqgfzy.top

strcmp(a, b) == 0
来源：http://yke.zdqjudy.top

[S07] C：数组遍历求和
来源：http://anu.shangyingyoupin.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dcz.nanxuanxn.top

[S08] C：动态内存分配与释放
来源：http://aii.sufxvd.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://duk.sjlbkw.cn

[S09] C：结构体定义与初始化
来源：http://oqb.fktsv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lka.ydzc1.top

[S10] C：指针与解引用
来源：http://xjb.tianlin.xyz

int *p = &a;  *p = 5;
来源：http://uxb.yanxiufei.cn

[S11] C：逐行读文件
来源：http://zag.smart0.xyz

FILE *f = fopen("a.txt", "r");
来源：http://yrq.yueranfly.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://luj.hongshengwenyu.top

fclose(f);
来源：http://eip.guowangkeji.top

[S12] C：写文件
来源：http://wht.epnwcf.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://alu.wangdashe.top

[S13] C：宏定义
来源：http://auj.iojbl.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ojp.jianghu66.top

[S14] C：枚举
来源：http://lki.hnqzz.top

enum Color { RED, GREEN, BLUE };
来源：http://bnt.xylfe.cn

[S15] C：类型转换
来源：http://dnj.kuanghao11.cn

(double) a / b
来源：http://rgg.dashuyun.cn

[S16] C：位操作置位
来源：http://hvq.zdbjq.cn


<!-- 参考信息 -->