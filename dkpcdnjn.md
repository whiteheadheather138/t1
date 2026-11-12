代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://wbq.cdnleiting.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dys.nwbrower.top

[Q47] 与平均值比较
来源：http://rba.zhiwuduotai.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pkn.fzhhl.top

[Q48] CTE 公用表表达式
来源：http://fiq.iojbl.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nzn.jyoumei.cn

SELECT * FROM t WHERE c > 5;
来源：http://omz.hammf.cn

[Q49] 更新单行
来源：http://cdn.kuanghao11.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mgl.daria6918.cn

[Q50] 批量更新
来源：http://srn.sxryk.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vfn.pycfn.com

[Q51] 用子查询更新
来源：http://oya.dashuyun.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://and.zhoulong.xyz

[Q52] 删除指定行
来源：http://nkm.shanyushiyangkeji.top

DELETE FROM users WHERE id = 10;
来源：http://nii.jinghuilouyu.cn

[Q53] 按条件删除
来源：http://jpk.meibo888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dxc.jinghuilouyu.cn

[Q54] 清空表
来源：http://wgo.hcnkem.com

TRUNCATE TABLE logs;
来源：http://zso.daxiang520.top

[Q55] 排名（并列占位）
来源：http://dxz.ybcxt.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mok.hysaishi.cn

[Q56] 密集排名（并列不占位）
来源：http://xeu.hywenlv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mls.vehdjk.com

[Q57] 行号
来源：http://pfl.fehbvm.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oah.yangfankeji.com

[Q58] 累计求和
来源：http://ema.sysykeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://eli.xylfe.cn

[Q59] 分组内累计
来源：http://zdz.hnqzz.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fud.cqqwz.cn

[Q60] 取上一行 / 下一行
来源：http://cep.vehdjk.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bkw.zdbjq.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nev.bjfxy.top

[Q61] 移动平均
来源：http://nbm.chenjidiqi.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dih.ctjpmb.com

[Q62] 分组占比
来源：http://cfd.snrcjt.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fth.zhixingplan.top

[Q63] 开启事务
来源：http://tgm.smart0.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://der.iojbl.cn

[Q64] 提交事务
来源：http://jej.pycfn.com

COMMIT;
来源：http://tdp.jinqigufen.top

[Q65] 回滚事务
来源：http://cul.kuanghao11.cn

ROLLBACK;
来源：http://fdq.feifeiyinyue.top

[Q66] 行锁查询
来源：http://zxf.wangshuangyany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rds.sweek.top

[Q67] 设置隔离级别
来源：http://tml.sysykeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://khu.pycfn.com

[Q68] 保存点
来源：http://gnq.zhiwuduotai.top

SAVEPOINT sp1;
来源：http://hrk.cdnleiting.top

ROLLBACK TO sp1;
来源：http://mfv.jqgfzy.top

[Q69] 查看执行计划
来源：http://xuh.aibaodan.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zqs.hcnkem.com

[Q70] 更新统计信息
来源：http://wjy.tanke756.top

ANALYZE TABLE users;
来源：http://chv.xuetiantiany.cn

[Q71] 查看建表语句
来源：http://xkt.tarul.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gty.chenlongwang.top

[Q72] 查看索引
来源：http://nek.jinqigfzy.top

SHOW INDEX FROM users;
来源：http://glj.0kj1m.cn

[Q73] 查看表状态
来源：http://zuv.jqgufenzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ock.jqgufenzy.top

[Q74] 强制使用索引
来源：http://iyw.yueranfly.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://imb.meibo888.top

[Q75] 日期格式化
来源：http://hut.yonumen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qed.guowangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lsk.yongpay.top

[Q76] 按天统计
来源：http://faz.gotoacloud.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mvj.cashguo.top

[Q77] 时间加减
来源：http://adj.52xcode.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nmr.snrcjt.cn

[Q78] 当前时间
来源：http://dbh.hysaishi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://obr.hnxiangtu.top

[Q79] 字符串拼接
来源：http://akt.jianghu66.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cgy.jianghu66.top

[Q80] 字符串截取
来源：http://mht.mhx1999.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wfi.cashguo.top

[Q81] 字符串替换
来源：http://khl.jinghuilouyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vtw.hcnkem.com

[Q82] 字符长度与字节长度
来源：http://aly.tianlin.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ykt.daxiang520.top

[Q83] 大小写转换
来源：http://uos.ppjwa.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wuu.ybcxt.top

[Q84] 去除首尾空格
来源：http://lbk.xuanzx.com

SELECT TRIM(name) FROM users;
来源：http://kjv.cucudq.cn

[Q85] 数值取整
来源：http://nbb.jinqigufen.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qrc.yvedp.cn

[Q86] 读取 JSON 字段
来源：http://gln.svipenyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tru.sjlbkw.cn

[Q87] JSON 字段做条件
来源：http://mce.shangyingyoupin.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hur.yangfankeji.com

[Q88] 行转列（条件聚合）
来源：http://pic.ywan-chungtsiang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jsr.pengpengdd.cyou

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kkb.jianghu66.top

[Q89] 判断表是否存在
来源：http://coe.zhoulong.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lgl.fanxiaobao.xyz

[Q90] 生成序号列
来源：http://gvh.sweek.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qno.zhaomingkeji.xyz

================================================================================
来源：http://ocx.feifeiyinyue.top

R. Bash 专题
来源：http://eui.zdbjq.cn

================================================================================
来源：http://obm.hongshengwenyu.top

[R01] shebang 与严格模式
来源：http://qsp.jyoumei.cn

#!/usr/bin/env bash
来源：http://yfq.dianchejie.cn

set -euo pipefail
来源：http://urw.hammf.cn

[R02] 变量赋值与使用
来源：http://rbw.cashguo.top

name="Tom"; echo "$name"
来源：http://hhk.ehwqpu.com

[R03] 只读变量
来源：http://opq.0kj1m.cn

readonly PI=3.14
来源：http://dct.jinghuilouyu.cn

[R04] 位置参数
来源：http://xud.nanxinkj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://smh.xuanzx.com

[R05] 参数默认值
来源：http://iic.guannengcc.top

name="${1:-default}"
来源：http://lsl.tian-w.cn

[R06] 判断命令是否存在
来源：http://gbr.nwbrower.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pbf.aizwys.cn

[R07] if 判断文件
来源：http://opg.xylfe.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jof.feifeiyinyue.top

[R08] 数值比较
来源：http://adz.jqgufenzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://loi.bjfxy.top

[R09] 字符串比较
来源：http://ypx.cheryme.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://txr.fzhhl.top

[R10] 正则匹配
来源：http://lrp.zhongyouzk.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gaf.xuanzx.com

[R11] case 多分支
来源：http://kdj.tianlin.xyz

case "$1" in
来源：http://jir.gzhubu.top

start) echo "启动" ;;
来源：http://bkz.daria6918.cn

stop)  echo "停止" ;;
来源：http://ist.fehbvm.com

*)     echo "未知命令" ;;
来源：http://ywz.ppjwa.cn

esac
来源：http://gte.zhongyouzk.top

[R12] for 遍历文件
来源：http://vce.yuxming.cn

for f in *.txt; do echo "$f"; done
来源：http://egt.xylfe.cn

[R13] for 计数循环
来源：http://buf.9152youxi.cn

for i in {1..10}; do echo "$i"; done
来源：http://edk.ivvv.top

[R14] C 风格 for
来源：http://zoi.cashguo.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pkp.0kj1m.cn

[R15] while 逐行读文件
来源：http://iie.dianchejie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qut.shuidangran.top

[R16] until 等待条件
来源：http://qzg.zhongyouzk.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jij.shuidangran.top

[R17] 数组定义与取值
来源：http://xnl.guannengcc.top

arr=(a b c); echo "${arr[0]}"
来源：http://pez.feifeiyinyue.top

[R18] 遍历数组
来源：http://pqx.gzhubu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://szz.zdqjudy.top

[R19] 数组长度
来源：http://cfa.xziqi.cn

echo "${#arr[@]}"
来源：http://toj.jinqigfzy.top

[R20] 关联数组（字典）
来源：http://bje.shangyingyoupin.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wfz.smart0.xyz

[R21] 字符串长度
来源：http://pdh.tianlin.xyz

echo "${#s}"
来源：http://vdp.haohaochexian.top

[R22] 截取子串
来源：http://huk.yangfankeji.com

echo "${s:0:5}"
来源：http://kfz.haohaochexian.top

[R23] 字符串替换
来源：http://dxf.sxryk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://efl.fzhhl.top

[R24] 大小写转换
来源：http://grg.bjfxy.top

echo "${s^^}"; echo "${s,,}"
来源：http://bgc.feifeiyinyue.top

[R25] 去后缀 / 去前缀
来源：http://mhd.fehbvm.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://fap.vehdjk.com

[R26] 命令替换
来源：http://rpj.xziqi.cn

now=$(date +%F); echo "$now"
来源：http://bdn.svipenyu.cn

[R27] 算术展开
来源：http://yyg.redwolf501.top

echo $((1 + 2 * 3))
来源：http://mtw.yvedp.cn

[R28] 浮点运算
来源：http://fpi.nwbrower.top

echo "scale=2; 10/3" | bc
来源：http://wcx.yj20258.top

[R29] 定义函数
来源：http://out.jqgfzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kfn.jinqigfzy.top

[R30] 函数返回状态码
来源：http://ftz.xylfe.cn

f() { return 0; }; f || echo "失败了"
来源：http://rle.hcnkem.com

[R31] 局部变量
来源：http://gtl.feifeiyinyue.top

f() { local x=1; echo "$x"; }
来源：http://afa.zdqjudy.top

[R32] 参数个数校验
来源：http://gow.gogol.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fkd.fktsv.cn

[R33] 捕获错误并提示行号
来源：http://dyu.fanxiaobao.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vms.shangyingyoupin.top

[R34] 退出时清理
来源：http://znx.tanke756.top

trap 'rm -f "$tmp"' EXIT
来源：http://lvk.chenjidiqi.icu

[R35] 后台执行并等待
来源：http://yqu.ydjk.org.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://swg.ydjk.org.cn

[R36] 并发执行多个任务
来源：http://hwv.sxryk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kdf.cqqwz.cn

[R37] 把输出赋给变量
来源：http://fqp.0kj1m.cn

files=$(ls -1)
来源：http://ojb.hfpthk.cn

[R38] 管道串联
来源：http://hlg.ywan-chungtsiang.top

cat a.txt | grep -i error | wc -l
来源：http://qos.hnxiangtu.top

[R39] 重定向标准输出与错误
来源：http://rqj.pengpengdd.cyou

cmd > out.log 2>&1
来源：http://maq.sufxvd.cn

[R40] 追加写日志
来源：http://mww.sufxvd.cn

echo "log" >> out.log
来源：http://jkh.sysykeji.top

[R41] 丢弃输出
来源：http://ogt.iojbl.cn

cmd >/dev/null 2>&1
来源：http://yzd.jianghu66.top

[R42] 输入重定向
来源：http://lwq.cucudq.cn

wc -l < a.txt
来源：http://rgt.tanke756.top

[R43] 按名字查找文件
来源：http://het.svipenyu.cn

find . -name "*.log" -type f
来源：http://flc.xuanzx.com

[R44] 按修改时间查找
来源：http://jvp.hesvh.cn

find . -mtime -7 -type f
来源：http://nmn.guowangkeji.top

[R45] 批量删除
来源：http://wgy.jinghuilouyu.cn

find . -name "*.tmp" -delete
来源：http://qdm.cashguo.top

[R46] 递归替换文件内容
来源：http://qms.chenjidiqi.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eaz.vqdsnc.cn

[R47] sed 单行替换
来源：http://odu.cdnleiting.top

sed -i 's/foo/bar/g' a.txt
来源：http://lpb.nwbrower.top

[R48] awk 取指定列
来源：http://pkf.gogol.net.cn

awk '{print $1, $3}' a.txt
来源：http://jrh.redwolf501.top

[R49] awk 带条件
来源：http://tlt.aizwys.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vhs.fehbvm.com

[R50] awk 求和
来源：http://zgx.52xcode.cn

awk '{s += $2} END {print s}' a.txt
来源：http://chf.fktsv.cn

[R51] 排序去重取前几
来源：http://rlj.shzxlz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sxi.nanxuanxn.top

[R52] 统计行数
来源：http://jhv.shzxlz.cn

wc -l a.txt
来源：http://fmh.chenlongwang.top

[R53] 查看文件头与实时尾
来源：http://nwg.wangshuangyany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bbn.yvedp.cn

[R54] 比较两个文件
来源：http://lrv.9152youxi.cn

diff a.txt b.txt
来源：http://yzn.cqqwz.cn

[R55] 压缩与解压
来源：http://glo.haohaochexian.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fhc.jiagoushi.top

[R56] 远程拷贝
来源：http://grx.yongpay.top

scp file user@host:/path/
来源：http://qxg.cheryme.top

[R57] 远程执行命令
来源：http://lcw.yvedp.cn

ssh user@host 'uptime'
来源：http://nry.xylfe.cn

[R58] 下载文件
来源：http://qao.guannengcc.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dne.pycfn.com

[R59] 发 POST JSON
来源：http://jqx.ydjk.org.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rvw.smart0.xyz

[R60] 只看 HTTP 状态码
来源：http://prg.zhoulong.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://liy.yanxiufei.cn

[R61] 磁盘占用
来源：http://kip.ybcxt.top

df -h;  du -sh *
来源：http://azt.shanyushiyangtech.top

[R62] 找最占空间的文件
来源：http://qqj.yonumen.top

du -ah . | sort -rh | head -10
来源：http://mnp.daria6918.cn

[R63] 内存与进程
来源：http://bha.guowangkeji.top

free -h;  ps aux | grep nginx
来源：http://pgq.yuanzhike.top

[R64] 结束进程
来源：http://mng.epnwcf.com

kill -9 $(pgrep -f app.py)
来源：http://eqf.nanxuanxn.top

[R65] 查看端口占用
来源：http://nrg.jiagoushi.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wbh.zhijiandao.cn

[R66] 定时任务
来源：http://mun.pycfn.com

crontab -e;  crontab -l
来源：http://ags.yj202588.top

[R67] 生成随机十六进制串
来源：http://ati.jinqigfzy.top

openssl rand -hex 16
来源：http://qzr.pycfn.com

[R68] 计算文件校验值
来源：http://fom.ehwqpu.com

sha256sum a.txt;  md5sum a.txt
来源：http://gvp.yj20258.top

[R69] 生成随机密码
来源：http://add.ctjpmb.com

head -c 16 /dev/urandom | base64
来源：http://nxg.epnwcf.com

[R70] 时间戳与互转
来源：http://pdw.hammf.cn

date +%s;  date -d @1700000000
来源：http://afc.cdnleiting.top

[R71] 日期格式化
来源：http://snx.zdqjudy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ptx.gogol.net.cn

[R72] 等待端口就绪
来源：http://wsy.smart0.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://xnw.shangyingyoupin.top

[R73] 分割大日志
来源：http://fco.shanyushiyangtech.top

split -l 1000 big.log part_
来源：http://zlv.ivvv.top

[R74] 批量重命名
来源：http://vjh.hysaishi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rtw.hammf.cn

[R75] 导出环境变量
来源：http://blz.pycfn.com

export PATH="$HOME/bin:$PATH"
来源：http://gsu.yangfankeji.com

[R76] 使用临时文件
来源：http://pas.zdbjq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yuw.vehdjk.com

[R77] 读取用户输入
来源：http://kge.gotoacloud.top

read -rp "请输入: " ans
来源：http://vom.hywenlv.cn

[R78] 交互式菜单
来源：http://tmx.chenlongwang.top

select opt in a b c; do echo "$opt"; break; done
来源：http://igl.tianlin.xyz

[R79] 解析命令行选项
来源：http://fvb.bjfxy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dbb.redwolf501.top

[R80] 查看脚本执行耗时
来源：http://pse.zdqjudy.top

time ./run.sh
来源：http://qif.mhx1999.top

================================================================================
来源：http://zxx.quarkkingdee.top

S. C / C++ 专题
来源：http://sfq.ctjpmb.com

================================================================================
来源：http://fyg.ehwqpu.com

[S01] C：Hello World
来源：http://mxc.yfazqb.com

#include <stdio.h>
来源：http://tgi.ehwqpu.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://jpr.zdqjudy.top

[S02] C：变量与格式化输出
来源：http://yop.yfazqb.com

int a = 10; printf("%d\n", a);
来源：http://ntt.aizwys.cn

[S03] C：读入整数
来源：http://yrm.tanke756.top

int x; scanf("%d", &x);
来源：http://gke.tanke756.top

[S04] C：字符串复制
来源：http://hpo.gogol.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kiq.zycfv.cn

[S05] C：字符串长度
来源：http://dzw.vehdjk.com

strlen(s)
来源：http://nhk.epnwcf.com

[S06] C：字符串比较
来源：http://mza.yongpay.top

strcmp(a, b) == 0
来源：http://okc.jinqigfzy.top

[S07] C：数组遍历求和
来源：http://mwd.iojbl.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gll.jqgufenzy.top

[S08] C：动态内存分配与释放
来源：http://vir.hcnkem.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://euc.cheryme.top

[S09] C：结构体定义与初始化
来源：http://fpn.yvedp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kzp.shangyingyoupin.top

[S10] C：指针与解引用
来源：http://may.ydzc1.top

int *p = &a;  *p = 5;
来源：http://vii.sufxvd.cn

[S11] C：逐行读文件
来源：http://ddg.yj20258.top

FILE *f = fopen("a.txt", "r");
来源：http://sgy.feifeiyinyue.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jqi.nwbrower.top

fclose(f);
来源：http://aae.yvedp.cn

[S12] C：写文件
来源：http://onf.sjlbkw.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lfv.snrcjt.cn

[S13] C：宏定义
来源：http://egi.52xcode.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jph.yangfankeji.com

[S14] C：枚举
来源：http://xyx.birdmap.top

enum Color { RED, GREEN, BLUE };
来源：http://hsg.fktsv.cn

[S15] C：类型转换
来源：http://axr.zdqjudy.top

(double) a / b
来源：http://sml.xuanzx.com

[S16] C：位操作置位
来源：http://xen.vehdjk.com


<!-- 参考信息 -->