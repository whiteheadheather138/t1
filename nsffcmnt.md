代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://beu.fktsv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xmr.xuanzx.com

[Q43] 标量子查询
来源：http://qit.hywenlv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://smw.ehwqpu.com

[Q44] IN 子查询
来源：http://txb.zhixingplan.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bua.gotoacloud.top

[Q45] EXISTS 判断存在
来源：http://awc.fengsongda.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dqa.hesvh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nll.jinqigfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fku.pengpengdd.cyou

[Q47] 与平均值比较
来源：http://gea.chenlongwang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dbj.xinyue.icu

[Q48] CTE 公用表表达式
来源：http://qix.jlsjyb.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dfq.hnxiangtu.top

SELECT * FROM t WHERE c > 5;
来源：http://nqh.hysaishi.cn

[Q49] 更新单行
来源：http://ken.yueranfly.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hcf.dashuyun.cn

[Q50] 批量更新
来源：http://ftz.nanxuanxn.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://akb.tian-w.cn

[Q51] 用子查询更新
来源：http://qnw.jyoumei.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://boy.birdmap.top

[Q52] 删除指定行
来源：http://ryl.feifeiyinyue.top

DELETE FROM users WHERE id = 10;
来源：http://wjz.fanxiaobao.xyz

[Q53] 按条件删除
来源：http://zav.fengsongda.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dqa.svipenyu.cn

[Q54] 清空表
来源：http://bvi.daxiang520.top

TRUNCATE TABLE logs;
来源：http://iyj.redwolf501.top

[Q55] 排名（并列占位）
来源：http://zvc.zhiwuduotai.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xum.quarkkingdee.top

[Q56] 密集排名（并列不占位）
来源：http://vty.tian-w.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rgz.zdqjudy.top

[Q57] 行号
来源：http://fip.yuxming.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vkd.zhengqikj.top

[Q58] 累计求和
来源：http://udt.sjlbkw.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nrg.shzxlz.cn

[Q59] 分组内累计
来源：http://bvu.vqdsnc.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kjf.hammf.cn

[Q60] 取上一行 / 下一行
来源：http://ehp.shuidangran.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rbl.sjlbkw.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://avo.jlsjyb.cn

[Q61] 移动平均
来源：http://hhx.daxiang520.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vpx.jianghu66.top

[Q62] 分组占比
来源：http://iet.chenlongwang.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rcu.zdbjq.cn

[Q63] 开启事务
来源：http://nqm.xingfuxueyuan.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://quy.hesvh.cn

[Q64] 提交事务
来源：http://zis.gzhubu.top

COMMIT;
来源：http://lis.sysykeji.top

[Q65] 回滚事务
来源：http://kex.yueranfly.top

ROLLBACK;
来源：http://dtq.daxiang520.top

[Q66] 行锁查询
来源：http://avd.sufxvd.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://agy.zhijiandao.cn

[Q67] 设置隔离级别
来源：http://zhw.yj202588.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rtb.tianlin.xyz

[Q68] 保存点
来源：http://lyl.wangdashe.top

SAVEPOINT sp1;
来源：http://ugn.hcnkem.com

ROLLBACK TO sp1;
来源：http://bfd.zycfv.cn

[Q69] 查看执行计划
来源：http://fmg.nwbrower.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gxa.shanyushiyangkeji.top

[Q70] 更新统计信息
来源：http://bep.zdbjq.cn

ANALYZE TABLE users;
来源：http://qjw.zhixingplan.top

[Q71] 查看建表语句
来源：http://nhj.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ilp.jlsjyb.cn

[Q72] 查看索引
来源：http://izj.pengpengdd.cyou

SHOW INDEX FROM users;
来源：http://sbj.guowangkeji.top

[Q73] 查看表状态
来源：http://omp.c1oappe.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wlv.yuanzhike.top

[Q74] 强制使用索引
来源：http://cfw.zhengqikj.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dlu.ywan-chungtsiang.top

[Q75] 日期格式化
来源：http://yze.tanke756.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vuz.jqgfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ttl.guannengcc.top

[Q76] 按天统计
来源：http://dpk.fanxiaobao.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wnt.shzxlz.cn

[Q77] 时间加减
来源：http://rem.jyoumei.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ird.gzhubu.top

[Q78] 当前时间
来源：http://myx.ctjpmb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oid.yanxiufei.cn

[Q79] 字符串拼接
来源：http://njm.yangfankeji.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xgt.yuxming.cn

[Q80] 字符串截取
来源：http://xnz.feifeiyinyue.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jjz.wangdashe.top

[Q81] 字符串替换
来源：http://ivh.hnqzz.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vfe.ivvv.top

[Q82] 字符长度与字节长度
来源：http://mky.sufxvd.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qvg.jinghuilouyu.cn

[Q83] 大小写转换
来源：http://uhx.gogol.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mjj.haohaochexian.top

[Q84] 去除首尾空格
来源：http://ohm.zycfv.cn

SELECT TRIM(name) FROM users;
来源：http://iyp.yonumen.top

[Q85] 数值取整
来源：http://qmg.hnqzz.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iiu.epnwcf.com

[Q86] 读取 JSON 字段
来源：http://eha.vehdjk.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kbb.chenlongwang.top

[Q87] JSON 字段做条件
来源：http://iqy.tanke756.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wsd.yueranfly.top

[Q88] 行转列（条件聚合）
来源：http://kiv.xuetiantiany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tne.ehwqpu.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ute.yonumen.top

[Q89] 判断表是否存在
来源：http://ied.9152youxi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ywq.cqqwz.cn

[Q90] 生成序号列
来源：http://gek.gogol.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://auc.vehdjk.com

================================================================================
来源：http://exl.hfpthk.cn

R. Bash 专题
来源：http://oln.ppjwa.cn

================================================================================
来源：http://ptb.yj20258.top

[R01] shebang 与严格模式
来源：http://elz.chenzaomai.com

#!/usr/bin/env bash
来源：http://gxf.cucudq.cn

set -euo pipefail
来源：http://aob.fanxiaobao.xyz

[R02] 变量赋值与使用
来源：http://fov.jyoumei.cn

name="Tom"; echo "$name"
来源：http://saz.bjfxy.top

[R03] 只读变量
来源：http://yte.yonumen.top

readonly PI=3.14
来源：http://vqh.snrcjt.cn

[R04] 位置参数
来源：http://src.gotoacloud.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://omi.0kj1m.cn

[R05] 参数默认值
来源：http://xnj.mhx1999.top

name="${1:-default}"
来源：http://yjo.uphjek.com

[R06] 判断命令是否存在
来源：http://ygp.xingfuxueyuan.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vuk.shangyingyoupin.top

[R07] if 判断文件
来源：http://hhb.pengpengdd.cyou

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tjw.vehdjk.com

[R08] 数值比较
来源：http://czi.jqgufenzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cmw.cucudq.cn

[R09] 字符串比较
来源：http://zny.yfazqb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xwp.zhongyouzk.top

[R10] 正则匹配
来源：http://iyx.hnxiangtu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jvg.shangyingyoupin.top

[R11] case 多分支
来源：http://vox.c1oappe.top

case "$1" in
来源：http://yfg.hesvh.cn

start) echo "启动" ;;
来源：http://avy.tianlin.xyz

stop)  echo "停止" ;;
来源：http://jzh.tianlin.xyz

*)     echo "未知命令" ;;
来源：http://tzm.shuidangran.top

esac
来源：http://ehm.ydzc1.top

[R12] for 遍历文件
来源：http://dum.yuanzhike.top

for f in *.txt; do echo "$f"; done
来源：http://fae.tarul.cn

[R13] for 计数循环
来源：http://gfw.hnxiangtu.top

for i in {1..10}; do echo "$i"; done
来源：http://xno.316326.xyz

[R14] C 风格 for
来源：http://shi.hysaishi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eey.yfazqb.com

[R15] while 逐行读文件
来源：http://yha.haohaochexian.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lih.ybcxt.top

[R16] until 等待条件
来源：http://rnl.ehwqpu.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pnr.hammf.cn

[R17] 数组定义与取值
来源：http://vpx.yvedp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gek.jlsjyb.cn

[R18] 遍历数组
来源：http://nuj.zhiwuduotai.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rvu.sjlbkw.cn

[R19] 数组长度
来源：http://kyu.gogol.net.cn

echo "${#arr[@]}"
来源：http://sfh.ppjwa.cn

[R20] 关联数组（字典）
来源：http://muq.yuxming.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kcf.chenzaomai.com

[R21] 字符串长度
来源：http://pub.pengpengdd.cyou

echo "${#s}"
来源：http://mby.jyoumei.cn

[R22] 截取子串
来源：http://aka.iojbl.cn

echo "${s:0:5}"
来源：http://lom.bbcook.cn

[R23] 字符串替换
来源：http://eot.yj20258.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wxj.52xcode.cn

[R24] 大小写转换
来源：http://ijr.shanyushiyangtech.top

echo "${s^^}"; echo "${s,,}"
来源：http://vpe.jiagoushi.top

[R25] 去后缀 / 去前缀
来源：http://wlx.aizwys.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://axm.52xcode.cn

[R26] 命令替换
来源：http://vem.nanxinkj.top

now=$(date +%F); echo "$now"
来源：http://ajq.zdqjudy.top

[R27] 算术展开
来源：http://tsl.zdbjq.cn

echo $((1 + 2 * 3))
来源：http://kpm.fengsongda.top

[R28] 浮点运算
来源：http://atf.cqqwz.cn

echo "scale=2; 10/3" | bc
来源：http://neu.zycfv.cn

[R29] 定义函数
来源：http://duk.jqgufenzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eyw.nwbrower.top

[R30] 函数返回状态码
来源：http://flq.jinqigfzy.top

f() { return 0; }; f || echo "失败了"
来源：http://uno.vqdsnc.cn

[R31] 局部变量
来源：http://fle.pycfn.com

f() { local x=1; echo "$x"; }
来源：http://hqp.xingfuxueyuan.xyz

[R32] 参数个数校验
来源：http://enm.tianlin.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vby.sufxvd.cn

[R33] 捕获错误并提示行号
来源：http://fzt.shzxlz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uav.hywenlv.cn

[R34] 退出时清理
来源：http://vol.shanyushiyangtech.top

trap 'rm -f "$tmp"' EXIT
来源：http://cpc.xinyue.icu

[R35] 后台执行并等待
来源：http://gzc.gzhubu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://bxq.jlsjyb.cn

[R36] 并发执行多个任务
来源：http://iue.hfpthk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://exc.hnqzz.top

[R37] 把输出赋给变量
来源：http://yjl.pengpengdd.cyou

files=$(ls -1)
来源：http://aoz.wangdashe.top

[R38] 管道串联
来源：http://ecv.svipenyu.cn

cat a.txt | grep -i error | wc -l
来源：http://vyj.yj20258.top

[R39] 重定向标准输出与错误
来源：http://prx.sxryk.cn

cmd > out.log 2>&1
来源：http://tnb.ivvv.top

[R40] 追加写日志
来源：http://ctc.jyoumei.cn

echo "log" >> out.log
来源：http://xbq.xziqi.cn

[R41] 丢弃输出
来源：http://cdc.jlsjyb.cn

cmd >/dev/null 2>&1
来源：http://hft.uphjek.com

[R42] 输入重定向
来源：http://kwh.ydzc1.top

wc -l < a.txt
来源：http://rku.bbcook.cn

[R43] 按名字查找文件
来源：http://tpj.dashuyun.cn

find . -name "*.log" -type f
来源：http://pjp.shuidangran.top

[R44] 按修改时间查找
来源：http://ody.jyoumei.cn

find . -mtime -7 -type f
来源：http://hui.hnxiangtu.top

[R45] 批量删除
来源：http://drc.shuidangran.top

find . -name "*.tmp" -delete
来源：http://ape.yvedp.cn

[R46] 递归替换文件内容
来源：http://vxz.yj20258.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xus.zdqjudy.top

[R47] sed 单行替换
来源：http://ncr.sufxvd.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tfo.shangyingyoupin.top

[R48] awk 取指定列
来源：http://iaq.sweek.top

awk '{print $1, $3}' a.txt
来源：http://aly.nwbrower.top

[R49] awk 带条件
来源：http://bva.iojbl.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://trt.nanxuanxn.top

[R50] awk 求和
来源：http://uwk.ctjpmb.com

awk '{s += $2} END {print s}' a.txt
来源：http://cwi.zdqjudy.top

[R51] 排序去重取前几
来源：http://xfi.0kj1m.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xwe.iojbl.cn

[R52] 统计行数
来源：http://uui.ydjk.org.cn

wc -l a.txt
来源：http://byl.yj20258.top

[R53] 查看文件头与实时尾
来源：http://wci.xylfe.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nnv.nwbrower.top

[R54] 比较两个文件
来源：http://dmk.cqqwz.cn

diff a.txt b.txt
来源：http://uek.ydzc1.top

[R55] 压缩与解压
来源：http://rxo.xziqi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ykq.ydzc1.top

[R56] 远程拷贝
来源：http://mpn.zhixingplan.top

scp file user@host:/path/
来源：http://vdr.hesvh.cn

[R57] 远程执行命令
来源：http://mhb.xinyue.icu

ssh user@host 'uptime'
来源：http://fch.jiagoushi.top

[R58] 下载文件
来源：http://fja.guannengcc.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rpz.guannengcc.top

[R59] 发 POST JSON
来源：http://zei.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dsi.yj20258888.top

[R60] 只看 HTTP 状态码
来源：http://mzs.zdqjudy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ira.havefunace.top

[R61] 磁盘占用
来源：http://oxo.hfpthk.cn

df -h;  du -sh *
来源：http://hul.yangfankeji.com

[R62] 找最占空间的文件
来源：http://rcf.xingfuxueyuan.xyz

du -ah . | sort -rh | head -10
来源：http://yjp.cqqwz.cn

[R63] 内存与进程
来源：http://rld.yfazqb.com

free -h;  ps aux | grep nginx
来源：http://cri.kuanghao11.cn

[R64] 结束进程
来源：http://dnn.shanyushiyangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://epp.hfpthk.cn

[R65] 查看端口占用
来源：http://toj.ydjk.org.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mei.tarul.cn

[R66] 定时任务
来源：http://esd.zhoulong.xyz

crontab -e;  crontab -l
来源：http://xbo.xinyue.icu

[R67] 生成随机十六进制串
来源：http://fxq.yfazqb.com

openssl rand -hex 16
来源：http://hju.daxiang520.top

[R68] 计算文件校验值
来源：http://cud.daxiang520.top

sha256sum a.txt;  md5sum a.txt
来源：http://kge.yongpay.top

[R69] 生成随机密码
来源：http://xso.hysaishi.cn

head -c 16 /dev/urandom | base64
来源：http://nup.jinqigufen.top

[R70] 时间戳与互转
来源：http://qye.dashuyun.cn

date +%s;  date -d @1700000000
来源：http://tgi.meibo888.top

[R71] 日期格式化
来源：http://czm.jyoumei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mcu.aizwys.cn

[R72] 等待端口就绪
来源：http://opt.hammf.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dfh.fktsv.cn

[R73] 分割大日志
来源：http://tfs.yj20258.top

split -l 1000 big.log part_
来源：http://nhw.bbcook.cn

[R74] 批量重命名
来源：http://hrm.mhx1999.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lsm.yj20258888.top

[R75] 导出环境变量
来源：http://dfp.fanxiaobao.xyz

export PATH="$HOME/bin:$PATH"
来源：http://zwn.dianchejie.cn

[R76] 使用临时文件
来源：http://bum.andypj.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pfn.epnwcf.com

[R77] 读取用户输入
来源：http://ayv.cheryme.top

read -rp "请输入: " ans
来源：http://osq.zhiwuduotai.top

[R78] 交互式菜单
来源：http://bzp.yj20258.top

select opt in a b c; do echo "$opt"; break; done
来源：http://pmk.yanxiufei.cn

[R79] 解析命令行选项
来源：http://psl.hywenlv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jep.jqgufenzy.top

[R80] 查看脚本执行耗时
来源：http://yuy.chenzaomai.com

time ./run.sh
来源：http://bbp.hnxiangtu.top

================================================================================
来源：http://hie.ppjwa.cn

S. C / C++ 专题
来源：http://dpk.iojbl.cn

================================================================================
来源：http://sgx.bjfxy.top

[S01] C：Hello World
来源：http://tdm.gogol.net.cn

#include <stdio.h>
来源：http://lmn.9152youxi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qki.zycfv.cn

[S02] C：变量与格式化输出
来源：http://vuk.uphjek.com

int a = 10; printf("%d\n", a);
来源：http://uhr.yongpay.top

[S03] C：读入整数
来源：http://tsc.cashguo.top

int x; scanf("%d", &x);
来源：http://wni.cucudq.cn

[S04] C：字符串复制
来源：http://acr.sweek.top

char dst[32]; strcpy(dst, "hi");
来源：http://jgi.sysykeji.top

[S05] C：字符串长度
来源：http://wam.zhaomingkeji.xyz

strlen(s)
来源：http://zed.guowangkeji.top

[S06] C：字符串比较
来源：http://aui.shanyushiyangkeji.top

strcmp(a, b) == 0
来源：http://iuz.gzhubu.top

[S07] C：数组遍历求和
来源：http://zqh.bbcook.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://smj.ctjpmb.com

[S08] C：动态内存分配与释放
来源：http://imd.pycfn.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://phn.ydzc1.top

[S09] C：结构体定义与初始化
来源：http://qjc.zhongyouzk.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yfy.hywenlv.cn

[S10] C：指针与解引用
来源：http://lcf.gzhubu.top

int *p = &a;  *p = 5;
来源：http://eqs.sysykeji.top

[S11] C：逐行读文件
来源：http://xoo.hammf.cn

FILE *f = fopen("a.txt", "r");
来源：http://xwj.yj20258888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://gda.xinyue.icu

fclose(f);
来源：http://iyw.wangshuangyany.cn

[S12] C：写文件
来源：http://ntz.tarul.cn


<!-- 参考信息 -->