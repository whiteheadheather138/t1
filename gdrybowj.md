代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ypf.ywan-chungtsiang.top

[Q50] 批量更新
来源：http://hgd.ivvv.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mbf.quarkkingdee.top

[Q51] 用子查询更新
来源：http://ggp.guowangkeji.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mqk.jyoumei.cn

[Q52] 删除指定行
来源：http://jol.nanxinkj.top

DELETE FROM users WHERE id = 10;
来源：http://vat.daria6918.cn

[Q53] 按条件删除
来源：http://ihv.chenjidiqi.icu

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zav.hesvh.cn

[Q54] 清空表
来源：http://kqd.meibo888.top

TRUNCATE TABLE logs;
来源：http://oqw.xylfe.cn

[Q55] 排名（并列占位）
来源：http://zbj.quarkkingdee.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qko.birdmap.top

[Q56] 密集排名（并列不占位）
来源：http://cmu.ydjk.org.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blb.birdmap.top

[Q57] 行号
来源：http://zxj.hnqzz.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jes.xuanzx.com

[Q58] 累计求和
来源：http://mqf.yanxiufei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zts.xuanzx.com

[Q59] 分组内累计
来源：http://awu.hfpthk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://htu.yongpay.top

[Q60] 取上一行 / 下一行
来源：http://svg.bbcook.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vlz.chenjidiqi.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vkf.zhijiandao.cn

[Q61] 移动平均
来源：http://kql.tianlin.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rxu.ehwqpu.com

[Q62] 分组占比
来源：http://fzs.jyoumei.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://grz.fengsongda.top

[Q63] 开启事务
来源：http://ycq.cheryme.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kde.316326.xyz

[Q64] 提交事务
来源：http://cec.chenlongwang.top

COMMIT;
来源：http://ljd.jinghuilouyu.cn

[Q65] 回滚事务
来源：http://heo.zdqjudy.top

ROLLBACK;
来源：http://hbo.9152youxi.cn

[Q66] 行锁查询
来源：http://rua.jyoumei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fdm.tian-w.cn

[Q67] 设置隔离级别
来源：http://hws.nanxinkj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dov.yj20258888.top

[Q68] 保存点
来源：http://okh.iojbl.cn

SAVEPOINT sp1;
来源：http://hew.yanxiufei.cn

ROLLBACK TO sp1;
来源：http://spt.svipenyu.cn

[Q69] 查看执行计划
来源：http://los.yfazqb.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sul.smart0.xyz

[Q70] 更新统计信息
来源：http://lrr.snrcjt.cn

ANALYZE TABLE users;
来源：http://iyj.vehdjk.com

[Q71] 查看建表语句
来源：http://ewq.fktsv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bua.zhijiandao.cn

[Q72] 查看索引
来源：http://yme.smart0.xyz

SHOW INDEX FROM users;
来源：http://jag.shzxlz.cn

[Q73] 查看表状态
来源：http://uzz.meibo888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://spw.cdnleiting.top

[Q74] 强制使用索引
来源：http://xqk.wangshuangyany.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lba.dianchejie.cn

[Q75] 日期格式化
来源：http://waf.tian-w.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ajr.svipenyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fbx.52xcode.cn

[Q76] 按天统计
来源：http://yvz.jqgufenzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nsv.hywenlv.cn

[Q77] 时间加减
来源：http://onj.ydjk.org.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://grx.zdqjudy.top

[Q78] 当前时间
来源：http://qej.chenlongwang.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ryh.fanxiaobao.xyz

[Q79] 字符串拼接
来源：http://lft.tianlin.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://whi.yj20258.top

[Q80] 字符串截取
来源：http://xvs.smart0.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dqc.cheryme.top

[Q81] 字符串替换
来源：http://evf.fzhhl.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://igz.zdbjq.cn

[Q82] 字符长度与字节长度
来源：http://xwn.dianchejie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://shm.meibo888.top

[Q83] 大小写转换
来源：http://ksc.zdbjq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rrw.nanxuanxn.top

[Q84] 去除首尾空格
来源：http://iqr.xylfe.cn

SELECT TRIM(name) FROM users;
来源：http://jzd.svipenyu.cn

[Q85] 数值取整
来源：http://yra.cheryme.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wzu.dianchejie.cn

[Q86] 读取 JSON 字段
来源：http://asc.shzxlz.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ltj.shangyingyoupin.top

[Q87] JSON 字段做条件
来源：http://qnf.aibaodan.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qvf.sxryk.cn

[Q88] 行转列（条件聚合）
来源：http://rlk.sjlbkw.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://egg.daria6918.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oqm.yj20258888.top

[Q89] 判断表是否存在
来源：http://tcv.bjfxy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uvw.fanxiaobao.xyz

[Q90] 生成序号列
来源：http://omq.zdqjudy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://smo.pycfn.com

================================================================================
来源：http://onw.zhiwuduotai.top

R. Bash 专题
来源：http://rdo.hywenlv.cn

================================================================================
来源：http://vws.mhx1999.top

[R01] shebang 与严格模式
来源：http://auh.vehdjk.com

#!/usr/bin/env bash
来源：http://xou.hnxiangtu.top

set -euo pipefail
来源：http://odl.sjlbkw.cn

[R02] 变量赋值与使用
来源：http://oaj.316326.xyz

name="Tom"; echo "$name"
来源：http://ruj.hywenlv.cn

[R03] 只读变量
来源：http://zur.iojbl.cn

readonly PI=3.14
来源：http://qfc.kuanghao11.cn

[R04] 位置参数
来源：http://mdw.tanke756.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gei.hysaishi.cn

[R05] 参数默认值
来源：http://hfs.yj20258888.top

name="${1:-default}"
来源：http://gfz.jyoumei.cn

[R06] 判断命令是否存在
来源：http://omt.xuanzx.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://njt.jianghu66.top

[R07] if 判断文件
来源：http://paq.fzhhl.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bqm.hnqzz.top

[R08] 数值比较
来源：http://heh.guannengcc.top

if (( a > b )); then echo "a 更大"; fi
来源：http://olk.gzhubu.top

[R09] 字符串比较
来源：http://kqm.jqgfzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zju.shanyushiyangtech.top

[R10] 正则匹配
来源：http://gvx.jianghu66.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yqi.sysykeji.top

[R11] case 多分支
来源：http://spe.kuanghao11.cn

case "$1" in
来源：http://pfe.yueranfly.top

start) echo "启动" ;;
来源：http://oac.sjlbkw.cn

stop)  echo "停止" ;;
来源：http://izf.ydjk.org.cn

*)     echo "未知命令" ;;
来源：http://wms.sysykeji.top

esac
来源：http://huy.gaohongyu789.top

[R12] for 遍历文件
来源：http://oko.zhixingplan.top

for f in *.txt; do echo "$f"; done
来源：http://mvn.hesvh.cn

[R13] for 计数循环
来源：http://mcj.jinqigufen.top

for i in {1..10}; do echo "$i"; done
来源：http://cck.xuanzx.com

[R14] C 风格 for
来源：http://zri.mhx1999.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ymw.gotoacloud.top

[R15] while 逐行读文件
来源：http://wym.ctjpmb.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lru.ivvv.top

[R16] until 等待条件
来源：http://vrm.dashuyun.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wtn.9152youxi.cn

[R17] 数组定义与取值
来源：http://ehy.yueranfly.top

arr=(a b c); echo "${arr[0]}"
来源：http://iyb.ivvv.top

[R18] 遍历数组
来源：http://voq.xuanzx.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ozw.zdbjq.cn

[R19] 数组长度
来源：http://wff.yangfankeji.com

echo "${#arr[@]}"
来源：http://qlq.gotoacloud.top

[R20] 关联数组（字典）
来源：http://huc.cdnleiting.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ytz.yueranfly.top

[R21] 字符串长度
来源：http://aze.yonumen.top

echo "${#s}"
来源：http://tpq.yj20258888.top

[R22] 截取子串
来源：http://iyr.zhiwuduotai.top

echo "${s:0:5}"
来源：http://vgo.cucudq.cn

[R23] 字符串替换
来源：http://qcs.xuanzx.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dwm.feifeiyinyue.top

[R24] 大小写转换
来源：http://egz.quarkkingdee.top

echo "${s^^}"; echo "${s,,}"
来源：http://ymd.redwolf501.top

[R25] 去后缀 / 去前缀
来源：http://anz.zhoulong.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://pcu.andypj.xyz

[R26] 命令替换
来源：http://olv.meibo888.top

now=$(date +%F); echo "$now"
来源：http://icl.gogol.net.cn

[R27] 算术展开
来源：http://abf.gzhubu.top

echo $((1 + 2 * 3))
来源：http://nhw.yangfankeji.com

[R28] 浮点运算
来源：http://vrg.chenlongwang.top

echo "scale=2; 10/3" | bc
来源：http://iit.jiagoushi.top

[R29] 定义函数
来源：http://jbo.hfpthk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://swb.chenzaomai.com

[R30] 函数返回状态码
来源：http://ypd.shangyingyoupin.top

f() { return 0; }; f || echo "失败了"
来源：http://kwp.hammf.cn

[R31] 局部变量
来源：http://lyk.ehwqpu.com

f() { local x=1; echo "$x"; }
来源：http://xvm.zhongyouzk.top

[R32] 参数个数校验
来源：http://kgx.ehwqpu.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bff.yj202588.top

[R33] 捕获错误并提示行号
来源：http://wmy.hnxiangtu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xgv.c1oappe.top

[R34] 退出时清理
来源：http://ouk.jlsjyb.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xvt.haohaochexian.top

[R35] 后台执行并等待
来源：http://brm.fktsv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oay.chenlongwang.top

[R36] 并发执行多个任务
来源：http://mhl.yj20258.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nfm.zhiwuduotai.top

[R37] 把输出赋给变量
来源：http://tqn.feifeiyinyue.top

files=$(ls -1)
来源：http://kni.guannengcc.top

[R38] 管道串联
来源：http://fkx.shuidangran.top

cat a.txt | grep -i error | wc -l
来源：http://spe.daria6918.cn

[R39] 重定向标准输出与错误
来源：http://niv.ydzc1.top

cmd > out.log 2>&1
来源：http://lws.wangdashe.top

[R40] 追加写日志
来源：http://xuc.fanxiaobao.xyz

echo "log" >> out.log
来源：http://miw.pycfn.com

[R41] 丢弃输出
来源：http://cdw.cdnleiting.top

cmd >/dev/null 2>&1
来源：http://men.gotoacloud.top

[R42] 输入重定向
来源：http://dgt.hongshengwenyu.top

wc -l < a.txt
来源：http://wte.shangyingyoupin.top

[R43] 按名字查找文件
来源：http://zra.shangyingyoupin.top

find . -name "*.log" -type f
来源：http://tcl.ydjk.org.cn

[R44] 按修改时间查找
来源：http://gen.yanxiufei.cn

find . -mtime -7 -type f
来源：http://hwp.smart0.xyz

[R45] 批量删除
来源：http://gbu.hammf.cn

find . -name "*.tmp" -delete
来源：http://xzr.zycfv.cn

[R46] 递归替换文件内容
来源：http://ibn.cqqwz.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://efi.chenzaomai.com

[R47] sed 单行替换
来源：http://quw.yongpay.top

sed -i 's/foo/bar/g' a.txt
来源：http://dyd.zhaomingkeji.xyz

[R48] awk 取指定列
来源：http://uhj.havefunace.top

awk '{print $1, $3}' a.txt
来源：http://mkj.sxryk.cn

[R49] awk 带条件
来源：http://vdy.cucudq.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tee.guannengcc.top

[R50] awk 求和
来源：http://uum.jianghu66.top

awk '{s += $2} END {print s}' a.txt
来源：http://mjy.shangyingyoupin.top

[R51] 排序去重取前几
来源：http://czt.yueranfly.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dah.andypj.xyz

[R52] 统计行数
来源：http://gwk.ywan-chungtsiang.top

wc -l a.txt
来源：http://zfy.snrcjt.cn

[R53] 查看文件头与实时尾
来源：http://xnk.iojbl.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baj.cheryme.top

[R54] 比较两个文件
来源：http://vut.vehdjk.com

diff a.txt b.txt
来源：http://ueg.sxryk.cn

[R55] 压缩与解压
来源：http://jsq.zhongyouzk.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hwm.feifeiyinyue.top

[R56] 远程拷贝
来源：http://pyo.jiagoushi.top

scp file user@host:/path/
来源：http://vqg.xziqi.cn

[R57] 远程执行命令
来源：http://lpz.chenjidiqi.icu

ssh user@host 'uptime'
来源：http://aok.ctjpmb.com

[R58] 下载文件
来源：http://oja.fanxiaobao.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dsk.gaohongyu789.top

[R59] 发 POST JSON
来源：http://lox.pengpengdd.cyou

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kxb.fktsv.cn

[R60] 只看 HTTP 状态码
来源：http://wlg.jinyuanbaomall.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cyv.nwbrower.top

[R61] 磁盘占用
来源：http://ohp.52xcode.cn

df -h;  du -sh *
来源：http://xok.jinyuanbaomall.cn

[R62] 找最占空间的文件
来源：http://jjl.zhoulong.xyz

du -ah . | sort -rh | head -10
来源：http://abu.jlsjyb.cn

[R63] 内存与进程
来源：http://yzw.jqgfzy.top

free -h;  ps aux | grep nginx
来源：http://tcf.zdqjudy.top

[R64] 结束进程
来源：http://aat.snrcjt.cn

kill -9 $(pgrep -f app.py)
来源：http://tnx.gzhubu.top

[R65] 查看端口占用
来源：http://wax.gogol.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uea.zhixingplan.top

[R66] 定时任务
来源：http://qqg.ppjwa.cn

crontab -e;  crontab -l
来源：http://xnp.yueranfly.top

[R67] 生成随机十六进制串
来源：http://ftj.svipenyu.cn

openssl rand -hex 16
来源：http://mbz.birdmap.top

[R68] 计算文件校验值
来源：http://bzp.shanyushiyangtech.top

sha256sum a.txt;  md5sum a.txt
来源：http://ltr.yonumen.top

[R69] 生成随机密码
来源：http://trc.yj20258.top

head -c 16 /dev/urandom | base64
来源：http://siv.daria6918.cn

[R70] 时间戳与互转
来源：http://wxw.gogol.net.cn

date +%s;  date -d @1700000000
来源：http://ajt.bjfxy.top

[R71] 日期格式化
来源：http://vze.vqdsnc.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://msu.tanke756.top

[R72] 等待端口就绪
来源：http://arl.andypj.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://ptd.gaohongyu789.top

[R73] 分割大日志
来源：http://lgc.wangdashe.top

split -l 1000 big.log part_
来源：http://sxr.cucudq.cn

[R74] 批量重命名
来源：http://jws.ppjwa.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ytn.fehbvm.com

[R75] 导出环境变量
来源：http://rsb.daxiang520.top

export PATH="$HOME/bin:$PATH"
来源：http://xth.chenjidiqi.icu

[R76] 使用临时文件
来源：http://bsw.cashguo.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nha.xinyue.icu

[R77] 读取用户输入
来源：http://gtd.dashuyun.cn

read -rp "请输入: " ans
来源：http://tck.cashguo.top

[R78] 交互式菜单
来源：http://syq.hnqzz.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jxg.jqgufenzy.top

[R79] 解析命令行选项
来源：http://lqg.yfazqb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tuy.svipenyu.cn

[R80] 查看脚本执行耗时
来源：http://jfr.guannengcc.top

time ./run.sh
来源：http://zuj.shangyingyoupin.top

================================================================================
来源：http://qnf.feifeiyinyue.top

S. C / C++ 专题
来源：http://myy.aibaodan.cn

================================================================================
来源：http://pfs.aizwys.cn

[S01] C：Hello World
来源：http://kqn.jianghu66.top

#include <stdio.h>
来源：http://nhr.jinghuilouyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tvq.aizwys.cn

[S02] C：变量与格式化输出
来源：http://uze.guannengcc.top

int a = 10; printf("%d\n", a);
来源：http://kyy.wangdashe.top

[S03] C：读入整数
来源：http://vml.mhx1999.top

int x; scanf("%d", &x);
来源：http://lwi.xziqi.cn

[S04] C：字符串复制
来源：http://ert.fanxiaobao.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://zbh.yj202588.top

[S05] C：字符串长度
来源：http://nly.sjlbkw.cn

strlen(s)
来源：http://xbm.ywan-chungtsiang.top

[S06] C：字符串比较
来源：http://nfo.yj20258888.top

strcmp(a, b) == 0
来源：http://pql.yj20258.top

[S07] C：数组遍历求和
来源：http://anc.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wfk.zhongyouzk.top

[S08] C：动态内存分配与释放
来源：http://sym.xziqi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yeq.kuanghao11.cn

[S09] C：结构体定义与初始化
来源：http://yfe.gzhubu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fld.haohaochexian.top

[S10] C：指针与解引用
来源：http://hlo.meibo888.top

int *p = &a;  *p = 5;
来源：http://yut.sysykeji.top

[S11] C：逐行读文件
来源：http://hyl.ivvv.top

FILE *f = fopen("a.txt", "r");
来源：http://itx.zhijiandao.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zdf.jinqigfzy.top

fclose(f);
来源：http://zqa.yueranfly.top

[S12] C：写文件
来源：http://qhj.hammf.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tqs.yvedp.cn

[S13] C：宏定义
来源：http://czk.c1oappe.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bbz.zhengqikj.top

[S14] C：枚举
来源：http://mbk.hesvh.cn

enum Color { RED, GREEN, BLUE };
来源：http://ylb.sysykeji.top

[S15] C：类型转换
来源：http://abj.cucudq.cn

(double) a / b
来源：http://jba.jlsjyb.cn

[S16] C：位操作置位
来源：http://lmx.cdnleiting.top

x |= (1 << 3);
来源：http://mmu.dashuyun.cn

[S17] C：安全拼接字符串
来源：http://wzq.yuxming.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://skw.fehbvm.com

[S18] C：命令行参数
来源：http://jld.guannengcc.top

int main(int argc, char **argv)
来源：http://abf.snrcjt.cn

[S19] C：快速排序
来源：http://lgx.hnxiangtu.top

qsort(a, n, sizeof(int), cmp);
来源：http://kaz.cdnleiting.top

[S20] C：二分查找
来源：http://sjf.zhiwuduotai.top


<!-- 参考信息 -->