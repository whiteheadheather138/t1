代发 wailian999

[Q48] CTE 公用表表达式
来源：http://fjj.jinghuilouyu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://glx.ctjpmb.com

SELECT * FROM t WHERE c > 5;
来源：http://nag.zhiwuduotai.top

[Q49] 更新单行
来源：http://nxs.ehwqpu.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://czq.zhiwuduotai.top

[Q50] 批量更新
来源：http://gux.epnwcf.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dnx.cheryme.top

[Q51] 用子查询更新
来源：http://ncb.hnqzz.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://urr.ybcxt.top

[Q52] 删除指定行
来源：http://wmm.hammf.cn

DELETE FROM users WHERE id = 10;
来源：http://svj.gotoacloud.top

[Q53] 按条件删除
来源：http://owy.kuanghao11.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eio.tian-w.cn

[Q54] 清空表
来源：http://cbo.gotoacloud.top

TRUNCATE TABLE logs;
来源：http://ksi.hesvh.cn

[Q55] 排名（并列占位）
来源：http://vcy.meibo888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nut.52xcode.cn

[Q56] 密集排名（并列不占位）
来源：http://fie.cheryme.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vkl.cheryme.top

[Q57] 行号
来源：http://gji.andypj.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pbh.zhongyouzk.top

[Q58] 累计求和
来源：http://izx.chenlongwang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://clo.tianlin.xyz

[Q59] 分组内累计
来源：http://nzu.iojbl.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jhv.zhiwuduotai.top

[Q60] 取上一行 / 下一行
来源：http://nll.nanxinkj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wis.hongshengwenyu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kfn.fengsongda.top

[Q61] 移动平均
来源：http://mfs.zhaomingkeji.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ypc.316326.xyz

[Q62] 分组占比
来源：http://tob.snrcjt.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pez.pengpengdd.cyou

[Q63] 开启事务
来源：http://kmq.cheryme.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dix.gaohongyu789.top

[Q64] 提交事务
来源：http://ztc.zdbjq.cn

COMMIT;
来源：http://tya.aibaodan.cn

[Q65] 回滚事务
来源：http://gbq.sufxvd.cn

ROLLBACK;
来源：http://xzc.sxryk.cn

[Q66] 行锁查询
来源：http://vnx.redwolf501.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nlh.dianchejie.cn

[Q67] 设置隔离级别
来源：http://ycn.jyoumei.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yui.zhijiandao.cn

[Q68] 保存点
来源：http://apd.andypj.xyz

SAVEPOINT sp1;
来源：http://yvz.iojbl.cn

ROLLBACK TO sp1;
来源：http://iiz.daria6918.cn

[Q69] 查看执行计划
来源：http://vpy.aibaodan.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xeu.yj20258.top

[Q70] 更新统计信息
来源：http://mic.fehbvm.com

ANALYZE TABLE users;
来源：http://jyf.hywenlv.cn

[Q71] 查看建表语句
来源：http://cfj.yuanzhike.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pvz.pengpengdd.cyou

[Q72] 查看索引
来源：http://cxu.nanxuanxn.top

SHOW INDEX FROM users;
来源：http://ssy.shzxlz.cn

[Q73] 查看表状态
来源：http://hxh.epnwcf.com

SHOW TABLE STATUS LIKE 'users';
来源：http://jfl.vehdjk.com

[Q74] 强制使用索引
来源：http://itd.guowangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://moc.yonumen.top

[Q75] 日期格式化
来源：http://dxe.yj20258888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dfp.meibo888.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://how.ehwqpu.com

[Q76] 按天统计
来源：http://xyh.yongpay.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://axq.sufxvd.cn

[Q77] 时间加减
来源：http://azn.chenjidiqi.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oee.wangshuangyany.cn

[Q78] 当前时间
来源：http://rwe.hywenlv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hxi.yuxming.cn

[Q79] 字符串拼接
来源：http://lip.havefunace.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uwz.yonumen.top

[Q80] 字符串截取
来源：http://mte.bjfxy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dno.sjlbkw.cn

[Q81] 字符串替换
来源：http://let.dashuyun.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tvn.guannengcc.top

[Q82] 字符长度与字节长度
来源：http://fiz.pengpengdd.cyou

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ead.52xcode.cn

[Q83] 大小写转换
来源：http://xez.hammf.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nyo.jqgfzy.top

[Q84] 去除首尾空格
来源：http://wph.hywenlv.cn

SELECT TRIM(name) FROM users;
来源：http://zqd.shanyushiyangkeji.top

[Q85] 数值取整
来源：http://jzt.wangshuangyany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wei.52xcode.cn

[Q86] 读取 JSON 字段
来源：http://xis.ydjk.org.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cho.xingfuxueyuan.xyz

[Q87] JSON 字段做条件
来源：http://qjj.0kj1m.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eve.hnxiangtu.top

[Q88] 行转列（条件聚合）
来源：http://kvk.zhengqikj.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sis.hnxiangtu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fqa.cucudq.cn

[Q89] 判断表是否存在
来源：http://vwi.zhixingplan.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bgh.guowangkeji.top

[Q90] 生成序号列
来源：http://hih.yj20258.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://skn.cdnleiting.top

================================================================================
来源：http://xfn.yvedp.cn

R. Bash 专题
来源：http://ift.ybcxt.top

================================================================================
来源：http://gbx.ctjpmb.com

[R01] shebang 与严格模式
来源：http://lht.c1oappe.top

#!/usr/bin/env bash
来源：http://occ.ydjk.org.cn

set -euo pipefail
来源：http://clp.havefunace.top

[R02] 变量赋值与使用
来源：http://qee.svipenyu.cn

name="Tom"; echo "$name"
来源：http://ybv.316326.xyz

[R03] 只读变量
来源：http://dpc.ctjpmb.com

readonly PI=3.14
来源：http://qih.daxiang520.top

[R04] 位置参数
来源：http://bua.cucudq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iaa.hongshengwenyu.top

[R05] 参数默认值
来源：http://yhd.chenlongwang.top

name="${1:-default}"
来源：http://tdd.xylfe.cn

[R06] 判断命令是否存在
来源：http://hyp.quarkkingdee.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bri.birdmap.top

[R07] if 判断文件
来源：http://brz.smart0.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mer.sweek.top

[R08] 数值比较
来源：http://mce.yvedp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pon.hysaishi.cn

[R09] 字符串比较
来源：http://rny.tian-w.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fjb.cqqwz.cn

[R10] 正则匹配
来源：http://ktc.andypj.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lrl.hesvh.cn

[R11] case 多分支
来源：http://nqt.ybcxt.top

case "$1" in
来源：http://phz.guowangkeji.top

start) echo "启动" ;;
来源：http://dnr.yanxiufei.cn

stop)  echo "停止" ;;
来源：http://ouq.cheryme.top

*)     echo "未知命令" ;;
来源：http://kud.yongpay.top

esac
来源：http://fjq.ywan-chungtsiang.top

[R12] for 遍历文件
来源：http://onm.yfazqb.com

for f in *.txt; do echo "$f"; done
来源：http://yfh.mhx1999.top

[R13] for 计数循环
来源：http://xpx.0kj1m.cn

for i in {1..10}; do echo "$i"; done
来源：http://dal.kuanghao11.cn

[R14] C 风格 for
来源：http://tlu.svipenyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://grj.ctjpmb.com

[R15] while 逐行读文件
来源：http://lqn.dianchejie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lyg.ywan-chungtsiang.top

[R16] until 等待条件
来源：http://aag.guannengcc.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://arj.yonumen.top

[R17] 数组定义与取值
来源：http://flj.52xcode.cn

arr=(a b c); echo "${arr[0]}"
来源：http://frw.9152youxi.cn

[R18] 遍历数组
来源：http://eto.jqgfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pgt.bbcook.cn

[R19] 数组长度
来源：http://pof.vehdjk.com

echo "${#arr[@]}"
来源：http://jip.sysykeji.top

[R20] 关联数组（字典）
来源：http://cwv.aibaodan.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://iko.sxryk.cn

[R21] 字符串长度
来源：http://byj.gotoacloud.top

echo "${#s}"
来源：http://mvt.guannengcc.top

[R22] 截取子串
来源：http://voe.ydjk.org.cn

echo "${s:0:5}"
来源：http://nmi.jqgfzy.top

[R23] 字符串替换
来源：http://llx.zdqjudy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zeo.tarul.cn

[R24] 大小写转换
来源：http://elz.sysykeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://gsx.ctjpmb.com

[R25] 去后缀 / 去前缀
来源：http://hfe.zhiwuduotai.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vjx.guannengcc.top

[R26] 命令替换
来源：http://qzb.jianghu66.top

now=$(date +%F); echo "$now"
来源：http://lpv.hywenlv.cn

[R27] 算术展开
来源：http://vbi.quarkkingdee.top

echo $((1 + 2 * 3))
来源：http://yjx.jlsjyb.cn

[R28] 浮点运算
来源：http://vtw.cqqwz.cn

echo "scale=2; 10/3" | bc
来源：http://zvw.nwbrower.top

[R29] 定义函数
来源：http://skb.feifeiyinyue.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eqy.mhx1999.top

[R30] 函数返回状态码
来源：http://eyk.svipenyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://lce.gogol.net.cn

[R31] 局部变量
来源：http://mhq.zdqjudy.top

f() { local x=1; echo "$x"; }
来源：http://faz.haohaochexian.top

[R32] 参数个数校验
来源：http://bpu.ppjwa.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kga.ppjwa.cn

[R33] 捕获错误并提示行号
来源：http://vlq.ydzc1.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wtc.xuanzx.com

[R34] 退出时清理
来源：http://gdp.ybcxt.top

trap 'rm -f "$tmp"' EXIT
来源：http://vur.yvedp.cn

[R35] 后台执行并等待
来源：http://qet.bbcook.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ala.jlsjyb.cn

[R36] 并发执行多个任务
来源：http://osm.uphjek.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lze.ybcxt.top

[R37] 把输出赋给变量
来源：http://cvz.jqgufenzy.top

files=$(ls -1)
来源：http://xbl.ywan-chungtsiang.top

[R38] 管道串联
来源：http://nrh.jinqigfzy.top

cat a.txt | grep -i error | wc -l
来源：http://gzi.chenjidiqi.icu

[R39] 重定向标准输出与错误
来源：http://icp.sxryk.cn

cmd > out.log 2>&1
来源：http://wag.zhoulong.xyz

[R40] 追加写日志
来源：http://bzz.fanxiaobao.xyz

echo "log" >> out.log
来源：http://lxq.nanxinkj.top

[R41] 丢弃输出
来源：http://mht.tian-w.cn

cmd >/dev/null 2>&1
来源：http://xaw.ehwqpu.com

[R42] 输入重定向
来源：http://huq.shangyingyoupin.top

wc -l < a.txt
来源：http://gai.xinyue.icu

[R43] 按名字查找文件
来源：http://oox.yongpay.top

find . -name "*.log" -type f
来源：http://pui.daxiang520.top

[R44] 按修改时间查找
来源：http://mgg.quarkkingdee.top

find . -mtime -7 -type f
来源：http://ild.fktsv.cn

[R45] 批量删除
来源：http://ydk.birdmap.top

find . -name "*.tmp" -delete
来源：http://hgc.dianchejie.cn

[R46] 递归替换文件内容
来源：http://jaj.daria6918.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vex.ppjwa.cn

[R47] sed 单行替换
来源：http://oia.cashguo.top

sed -i 's/foo/bar/g' a.txt
来源：http://zzu.tarul.cn

[R48] awk 取指定列
来源：http://ens.gzhubu.top

awk '{print $1, $3}' a.txt
来源：http://rtz.yueranfly.top

[R49] awk 带条件
来源：http://ufx.fzhhl.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tcr.yvedp.cn

[R50] awk 求和
来源：http://brs.vqdsnc.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sea.cdnleiting.top

[R51] 排序去重取前几
来源：http://njq.fzhhl.top

sort a.txt | uniq -c | sort -rn | head
来源：http://iel.xylfe.cn

[R52] 统计行数
来源：http://vbm.aibaodan.cn

wc -l a.txt
来源：http://uve.tianlin.xyz

[R53] 查看文件头与实时尾
来源：http://vch.pycfn.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ajn.gzhubu.top

[R54] 比较两个文件
来源：http://rjt.fktsv.cn

diff a.txt b.txt
来源：http://dbu.ybcxt.top

[R55] 压缩与解压
来源：http://lwz.52xcode.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bgo.shuidangran.top

[R56] 远程拷贝
来源：http://pas.wangdashe.top

scp file user@host:/path/
来源：http://bme.zhixingplan.top

[R57] 远程执行命令
来源：http://hvv.zdqjudy.top

ssh user@host 'uptime'
来源：http://gsm.wangdashe.top

[R58] 下载文件
来源：http://chj.zdqjudy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mtb.52xcode.cn

[R59] 发 POST JSON
来源：http://qix.c1oappe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vem.zhongyouzk.top

[R60] 只看 HTTP 状态码
来源：http://kcl.hywenlv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://brq.cheryme.top

[R61] 磁盘占用
来源：http://ncq.sysykeji.top

df -h;  du -sh *
来源：http://xds.316326.xyz

[R62] 找最占空间的文件
来源：http://cdq.fengsongda.top

du -ah . | sort -rh | head -10
来源：http://afn.0kj1m.cn

[R63] 内存与进程
来源：http://wxx.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://bxw.uphjek.com

[R64] 结束进程
来源：http://gar.pengpengdd.cyou

kill -9 $(pgrep -f app.py)
来源：http://due.wangshuangyany.cn

[R65] 查看端口占用
来源：http://hah.feifeiyinyue.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ukv.daria6918.cn

[R66] 定时任务
来源：http://klm.cashguo.top

crontab -e;  crontab -l
来源：http://oay.fktsv.cn

[R67] 生成随机十六进制串
来源：http://wpl.snrcjt.cn

openssl rand -hex 16
来源：http://pmu.9152youxi.cn

[R68] 计算文件校验值
来源：http://odv.jqgufenzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://lkn.aibaodan.cn

[R69] 生成随机密码
来源：http://wvo.zhengqikj.top

head -c 16 /dev/urandom | base64
来源：http://edd.yongpay.top

[R70] 时间戳与互转
来源：http://bqh.dianchejie.cn

date +%s;  date -d @1700000000
来源：http://ycc.zdqjudy.top

[R71] 日期格式化
来源：http://hhw.wangdashe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kck.sweek.top

[R72] 等待端口就绪
来源：http://lzg.mhx1999.top

until nc -z localhost 3306; do sleep 1; done
来源：http://xca.hfpthk.cn

[R73] 分割大日志
来源：http://jnk.ctjpmb.com

split -l 1000 big.log part_
来源：http://nnc.chenzaomai.com

[R74] 批量重命名
来源：http://klm.yj20258.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://swt.svipenyu.cn

[R75] 导出环境变量
来源：http://hxj.yuxming.cn

export PATH="$HOME/bin:$PATH"
来源：http://wjc.zhixingplan.top

[R76] 使用临时文件
来源：http://uvt.zhixingplan.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://adv.cucudq.cn

[R77] 读取用户输入
来源：http://hsv.snrcjt.cn

read -rp "请输入: " ans
来源：http://kin.jianghu66.top

[R78] 交互式菜单
来源：http://xfz.jyoumei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nys.sufxvd.cn

[R79] 解析命令行选项
来源：http://cor.jinqigufen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mfz.ehwqpu.com

[R80] 查看脚本执行耗时
来源：http://lwb.epnwcf.com

time ./run.sh
来源：http://cwq.epnwcf.com

================================================================================
来源：http://ngp.pycfn.com

S. C / C++ 专题
来源：http://hsn.fehbvm.com

================================================================================
来源：http://dye.ydzc1.top

[S01] C：Hello World
来源：http://jnx.zdqjudy.top

#include <stdio.h>
来源：http://mxq.uphjek.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://ken.xuanzx.com

[S02] C：变量与格式化输出
来源：http://djg.pycfn.com

int a = 10; printf("%d\n", a);
来源：http://gjy.pengpengdd.cyou

[S03] C：读入整数
来源：http://hsb.smart0.xyz

int x; scanf("%d", &x);
来源：http://gwy.chenjidiqi.icu

[S04] C：字符串复制
来源：http://fqk.yonumen.top

char dst[32]; strcpy(dst, "hi");
来源：http://pmf.dashuyun.cn

[S05] C：字符串长度
来源：http://ibe.bjfxy.top

strlen(s)
来源：http://ryw.hongshengwenyu.top

[S06] C：字符串比较
来源：http://mdr.jiagoushi.top

strcmp(a, b) == 0
来源：http://hxb.wangshuangyany.cn

[S07] C：数组遍历求和
来源：http://tgd.zhaomingkeji.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://efl.jinghuilouyu.cn

[S08] C：动态内存分配与释放
来源：http://urh.52xcode.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qzu.aibaodan.cn

[S09] C：结构体定义与初始化
来源：http://bjw.chenlongwang.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rfh.wangshuangyany.cn

[S10] C：指针与解引用
来源：http://gel.jqgfzy.top

int *p = &a;  *p = 5;
来源：http://wqo.birdmap.top

[S11] C：逐行读文件
来源：http://quh.yanxiufei.cn

FILE *f = fopen("a.txt", "r");
来源：http://oie.jinghuilouyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ylu.sjlbkw.cn

fclose(f);
来源：http://gfy.yangfankeji.com

[S12] C：写文件
来源：http://fgq.xziqi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lkc.ydjk.org.cn

[S13] C：宏定义
来源：http://sxi.guannengcc.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cnp.shuidangran.top

[S14] C：枚举
来源：http://mtb.yongpay.top

enum Color { RED, GREEN, BLUE };
来源：http://xzl.52xcode.cn

[S15] C：类型转换
来源：http://fkk.shangyingyoupin.top

(double) a / b
来源：http://nmi.guowangkeji.top

[S16] C：位操作置位
来源：http://chc.316326.xyz

x |= (1 << 3);
来源：http://iub.nwbrower.top

[S17] C：安全拼接字符串
来源：http://lut.smart0.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cyd.jqgfzy.top

[S18] C：命令行参数
来源：http://iqg.wangshuangyany.cn


<!-- 参考信息 -->