代发 wailian999

[Q48] CTE 公用表表达式
来源：http://ond.chenlongwang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wcm.bjfxy.top

SELECT * FROM t WHERE c > 5;
来源：http://ctp.feifeiyinyue.top

[Q49] 更新单行
来源：http://xrx.yueranfly.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xxu.nwbrower.top

[Q50] 批量更新
来源：http://ror.xingfuxueyuan.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ojt.nwbrower.top

[Q51] 用子查询更新
来源：http://ztj.chenjidiqi.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ygp.tarul.cn

[Q52] 删除指定行
来源：http://wcg.jinghuilouyu.cn

DELETE FROM users WHERE id = 10;
来源：http://dfw.iojbl.cn

[Q53] 按条件删除
来源：http://smd.zhixingplan.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lpe.jqgfzy.top

[Q54] 清空表
来源：http://dus.daxiang520.top

TRUNCATE TABLE logs;
来源：http://msj.pengpengdd.cyou

[Q55] 排名（并列占位）
来源：http://oab.cucudq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://eho.shanyushiyangtech.top

[Q56] 密集排名（并列不占位）
来源：http://onm.yueranfly.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ieq.yfazqb.com

[Q57] 行号
来源：http://iki.haohaochexian.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://azh.quarkkingdee.top

[Q58] 累计求和
来源：http://ygu.hongshengwenyu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ykn.hnqzz.top

[Q59] 分组内累计
来源：http://omn.yuanzhike.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pqh.zycfv.cn

[Q60] 取上一行 / 下一行
来源：http://yvz.52xcode.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mkn.hysaishi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://odq.xuanzx.com

[Q61] 移动平均
来源：http://llb.hnqzz.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mge.yongpay.top

[Q62] 分组占比
来源：http://jbu.chenzaomai.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wtz.birdmap.top

[Q63] 开启事务
来源：http://gym.hfpthk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ybg.hammf.cn

[Q64] 提交事务
来源：http://dmt.yangfankeji.com

COMMIT;
来源：http://piz.ppjwa.cn

[Q65] 回滚事务
来源：http://pdp.hongshengwenyu.top

ROLLBACK;
来源：http://kdd.ehwqpu.com

[Q66] 行锁查询
来源：http://zqs.yanxiufei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yla.yuxming.cn

[Q67] 设置隔离级别
来源：http://vip.andypj.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rsx.sweek.top

[Q68] 保存点
来源：http://byb.tianlin.xyz

SAVEPOINT sp1;
来源：http://ayf.epnwcf.com

ROLLBACK TO sp1;
来源：http://uyw.sysykeji.top

[Q69] 查看执行计划
来源：http://yip.bjfxy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gml.cdnleiting.top

[Q70] 更新统计信息
来源：http://vfg.0kj1m.cn

ANALYZE TABLE users;
来源：http://riz.nanxuanxn.top

[Q71] 查看建表语句
来源：http://ios.sjlbkw.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kio.havefunace.top

[Q72] 查看索引
来源：http://jxx.hfpthk.cn

SHOW INDEX FROM users;
来源：http://ysx.fktsv.cn

[Q73] 查看表状态
来源：http://yth.gaohongyu789.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wpb.xuetiantiany.cn

[Q74] 强制使用索引
来源：http://zom.dashuyun.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nrd.yuxming.cn

[Q75] 日期格式化
来源：http://mpk.svipenyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ejm.yvedp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yrd.fzhhl.top

[Q76] 按天统计
来源：http://pky.yonumen.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tak.havefunace.top

[Q77] 时间加减
来源：http://mcq.iojbl.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ram.svipenyu.cn

[Q78] 当前时间
来源：http://obx.aizwys.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zfv.gotoacloud.top

[Q79] 字符串拼接
来源：http://rob.vqdsnc.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ihe.daxiang520.top

[Q80] 字符串截取
来源：http://dlx.zhixingplan.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dgm.tianlin.xyz

[Q81] 字符串替换
来源：http://zut.jinqigufen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sor.chenjidiqi.icu

[Q82] 字符长度与字节长度
来源：http://eek.jinyuanbaomall.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://srs.tianlin.xyz

[Q83] 大小写转换
来源：http://doz.zhoulong.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tym.yonumen.top

[Q84] 去除首尾空格
来源：http://fzg.gotoacloud.top

SELECT TRIM(name) FROM users;
来源：http://leb.nanxinkj.top

[Q85] 数值取整
来源：http://fum.hesvh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fud.uphjek.com

[Q86] 读取 JSON 字段
来源：http://uwr.pengpengdd.cyou

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qtj.xuanzx.com

[Q87] JSON 字段做条件
来源：http://dob.redwolf501.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qiv.guannengcc.top

[Q88] 行转列（条件聚合）
来源：http://ply.ybcxt.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vem.yj202588.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nlb.daxiang520.top

[Q89] 判断表是否存在
来源：http://mtc.bjfxy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://igc.xuanzx.com

[Q90] 生成序号列
来源：http://pec.shuidangran.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ekz.cheryme.top

================================================================================
来源：http://sjz.ywan-chungtsiang.top

R. Bash 专题
来源：http://pzz.jqgfzy.top

================================================================================
来源：http://qtw.xingfuxueyuan.xyz

[R01] shebang 与严格模式
来源：http://umj.gogol.net.cn

#!/usr/bin/env bash
来源：http://nmk.hammf.cn

set -euo pipefail
来源：http://grp.gaohongyu789.top

[R02] 变量赋值与使用
来源：http://pzt.chenlongwang.top

name="Tom"; echo "$name"
来源：http://dis.nanxuanxn.top

[R03] 只读变量
来源：http://yaj.feifeiyinyue.top

readonly PI=3.14
来源：http://cjp.316326.xyz

[R04] 位置参数
来源：http://kcm.tanke756.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cua.sweek.top

[R05] 参数默认值
来源：http://cuo.chenzaomai.com

name="${1:-default}"
来源：http://bvp.shanyushiyangtech.top

[R06] 判断命令是否存在
来源：http://lef.316326.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oqk.fktsv.cn

[R07] if 判断文件
来源：http://pcz.0kj1m.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://prd.hammf.cn

[R08] 数值比较
来源：http://csx.9152youxi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vdj.yueranfly.top

[R09] 字符串比较
来源：http://rrh.jlsjyb.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vba.jinghuilouyu.cn

[R10] 正则匹配
来源：http://toa.yvedp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://foy.shuidangran.top

[R11] case 多分支
来源：http://rcn.52xcode.cn

case "$1" in
来源：http://jtq.zhijiandao.cn

start) echo "启动" ;;
来源：http://zjy.gotoacloud.top

stop)  echo "停止" ;;
来源：http://hcc.svipenyu.cn

*)     echo "未知命令" ;;
来源：http://jlw.zdbjq.cn

esac
来源：http://kkz.ydjk.org.cn

[R12] for 遍历文件
来源：http://svc.kuanghao11.cn

for f in *.txt; do echo "$f"; done
来源：http://wcz.ctjpmb.com

[R13] for 计数循环
来源：http://oqm.nwbrower.top

for i in {1..10}; do echo "$i"; done
来源：http://cey.tianlin.xyz

[R14] C 风格 for
来源：http://idf.shanyushiyangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yta.jinyuanbaomall.cn

[R15] while 逐行读文件
来源：http://jhl.cqqwz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://shj.gaohongyu789.top

[R16] until 等待条件
来源：http://nld.yvedp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iet.bjfxy.top

[R17] 数组定义与取值
来源：http://zmv.xinyue.icu

arr=(a b c); echo "${arr[0]}"
来源：http://pzi.tian-w.cn

[R18] 遍历数组
来源：http://bvv.zhoulong.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kvb.jiagoushi.top

[R19] 数组长度
来源：http://bry.wangshuangyany.cn

echo "${#arr[@]}"
来源：http://spg.yj20258888.top

[R20] 关联数组（字典）
来源：http://bzd.sweek.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zrk.shzxlz.cn

[R21] 字符串长度
来源：http://giy.fzhhl.top

echo "${#s}"
来源：http://enl.kuanghao11.cn

[R22] 截取子串
来源：http://kcu.chenlongwang.top

echo "${s:0:5}"
来源：http://rlr.wangshuangyany.cn

[R23] 字符串替换
来源：http://aeg.pengpengdd.cyou

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hyc.fanxiaobao.xyz

[R24] 大小写转换
来源：http://xkw.iojbl.cn

echo "${s^^}"; echo "${s,,}"
来源：http://emf.pycfn.com

[R25] 去后缀 / 去前缀
来源：http://anb.chenjidiqi.icu

echo "${f%.txt}"; echo "${f#./}"
来源：http://jwi.sjlbkw.cn

[R26] 命令替换
来源：http://xzu.dianchejie.cn

now=$(date +%F); echo "$now"
来源：http://jnm.jinqigfzy.top

[R27] 算术展开
来源：http://xvx.gaohongyu789.top

echo $((1 + 2 * 3))
来源：http://equ.hfpthk.cn

[R28] 浮点运算
来源：http://fal.xingfuxueyuan.xyz

echo "scale=2; 10/3" | bc
来源：http://lje.gotoacloud.top

[R29] 定义函数
来源：http://vap.wangdashe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fxn.jinqigufen.top

[R30] 函数返回状态码
来源：http://wgf.iojbl.cn

f() { return 0; }; f || echo "失败了"
来源：http://vpc.ywan-chungtsiang.top

[R31] 局部变量
来源：http://jdk.nwbrower.top

f() { local x=1; echo "$x"; }
来源：http://mjy.jinyuanbaomall.cn

[R32] 参数个数校验
来源：http://rod.xinyue.icu

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rnh.chenzaomai.com

[R33] 捕获错误并提示行号
来源：http://qsm.yonumen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://khu.xuanzx.com

[R34] 退出时清理
来源：http://vbq.fktsv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hns.tian-w.cn

[R35] 后台执行并等待
来源：http://duh.zycfv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hrv.jiagoushi.top

[R36] 并发执行多个任务
来源：http://ysa.sweek.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://aos.kuanghao11.cn

[R37] 把输出赋给变量
来源：http://azm.yueranfly.top

files=$(ls -1)
来源：http://egb.jyoumei.cn

[R38] 管道串联
来源：http://ojf.yangfankeji.com

cat a.txt | grep -i error | wc -l
来源：http://axt.yanxiufei.cn

[R39] 重定向标准输出与错误
来源：http://lxz.jinqigfzy.top

cmd > out.log 2>&1
来源：http://qad.9152youxi.cn

[R40] 追加写日志
来源：http://rbe.cheryme.top

echo "log" >> out.log
来源：http://tkr.ybcxt.top

[R41] 丢弃输出
来源：http://ysw.gzhubu.top

cmd >/dev/null 2>&1
来源：http://xjs.snrcjt.cn

[R42] 输入重定向
来源：http://mqv.jiagoushi.top

wc -l < a.txt
来源：http://tlq.gzhubu.top

[R43] 按名字查找文件
来源：http://swz.fengsongda.top

find . -name "*.log" -type f
来源：http://aob.sufxvd.cn

[R44] 按修改时间查找
来源：http://eur.jyoumei.cn

find . -mtime -7 -type f
来源：http://eyx.hfpthk.cn

[R45] 批量删除
来源：http://ewp.jiagoushi.top

find . -name "*.tmp" -delete
来源：http://qnl.pengpengdd.cyou

[R46] 递归替换文件内容
来源：http://gme.nanxinkj.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bkl.uphjek.com

[R47] sed 单行替换
来源：http://pcj.andypj.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://obk.zhengqikj.top

[R48] awk 取指定列
来源：http://rsd.xziqi.cn

awk '{print $1, $3}' a.txt
来源：http://pvu.yj20258.top

[R49] awk 带条件
来源：http://yza.52xcode.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mdw.shanyushiyangtech.top

[R50] awk 求和
来源：http://xdm.fzhhl.top

awk '{s += $2} END {print s}' a.txt
来源：http://rez.aibaodan.cn

[R51] 排序去重取前几
来源：http://hpv.dashuyun.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pzh.jqgfzy.top

[R52] 统计行数
来源：http://asc.c1oappe.top

wc -l a.txt
来源：http://hyt.hysaishi.cn

[R53] 查看文件头与实时尾
来源：http://rgf.pengpengdd.cyou

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://omn.birdmap.top

[R54] 比较两个文件
来源：http://tol.daria6918.cn

diff a.txt b.txt
来源：http://ugc.fengsongda.top

[R55] 压缩与解压
来源：http://twx.havefunace.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zpd.yonumen.top

[R56] 远程拷贝
来源：http://ppl.yueranfly.top

scp file user@host:/path/
来源：http://dta.hcnkem.com

[R57] 远程执行命令
来源：http://rzy.xinyue.icu

ssh user@host 'uptime'
来源：http://pec.dianchejie.cn

[R58] 下载文件
来源：http://sxv.cucudq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sdb.vehdjk.com

[R59] 发 POST JSON
来源：http://nkg.zhixingplan.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rer.bbcook.cn

[R60] 只看 HTTP 状态码
来源：http://ken.jqgfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vtl.cdnleiting.top

[R61] 磁盘占用
来源：http://cbp.pengpengdd.cyou

df -h;  du -sh *
来源：http://ock.jqgfzy.top

[R62] 找最占空间的文件
来源：http://crv.zdqjudy.top

du -ah . | sort -rh | head -10
来源：http://bep.0kj1m.cn

[R63] 内存与进程
来源：http://lob.daxiang520.top

free -h;  ps aux | grep nginx
来源：http://qwb.daxiang520.top

[R64] 结束进程
来源：http://tyb.hfpthk.cn

kill -9 $(pgrep -f app.py)
来源：http://wao.gotoacloud.top

[R65] 查看端口占用
来源：http://cil.fanxiaobao.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bor.jinqigfzy.top

[R66] 定时任务
来源：http://jyz.zdqjudy.top

crontab -e;  crontab -l
来源：http://zra.gogol.net.cn

[R67] 生成随机十六进制串
来源：http://wut.tian-w.cn

openssl rand -hex 16
来源：http://foj.iojbl.cn

[R68] 计算文件校验值
来源：http://hwv.yuxming.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vnu.zhiwuduotai.top

[R69] 生成随机密码
来源：http://ihj.meibo888.top

head -c 16 /dev/urandom | base64
来源：http://rif.shanyushiyangkeji.top

[R70] 时间戳与互转
来源：http://wjf.tanke756.top

date +%s;  date -d @1700000000
来源：http://rky.fktsv.cn

[R71] 日期格式化
来源：http://hmy.nwbrower.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wcr.ppjwa.cn

[R72] 等待端口就绪
来源：http://rlt.andypj.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://tbd.zhengqikj.top

[R73] 分割大日志
来源：http://ehd.zdbjq.cn

split -l 1000 big.log part_
来源：http://yhy.jinqigufen.top

[R74] 批量重命名
来源：http://hwb.cdnleiting.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vrm.gotoacloud.top

[R75] 导出环境变量
来源：http://dnw.quarkkingdee.top

export PATH="$HOME/bin:$PATH"
来源：http://qjc.snrcjt.cn

[R76] 使用临时文件
来源：http://fri.hammf.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jqs.tanke756.top

[R77] 读取用户输入
来源：http://xdm.jianghu66.top

read -rp "请输入: " ans
来源：http://fxt.guowangkeji.top

[R78] 交互式菜单
来源：http://ffc.xingfuxueyuan.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://dws.sjlbkw.cn

[R79] 解析命令行选项
来源：http://lvv.9152youxi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zng.xylfe.cn

[R80] 查看脚本执行耗时
来源：http://gyx.hammf.cn

time ./run.sh
来源：http://fub.fktsv.cn

================================================================================
来源：http://deu.gogol.net.cn

S. C / C++ 专题
来源：http://mbn.hywenlv.cn

================================================================================
来源：http://cvm.jinqigufen.top

[S01] C：Hello World
来源：http://wgh.cqqwz.cn

#include <stdio.h>
来源：http://utf.zhongyouzk.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wfg.sjlbkw.cn

[S02] C：变量与格式化输出
来源：http://mjo.jiagoushi.top

int a = 10; printf("%d\n", a);
来源：http://gdj.vqdsnc.cn

[S03] C：读入整数
来源：http://pks.andypj.xyz

int x; scanf("%d", &x);
来源：http://kea.xziqi.cn

[S04] C：字符串复制
来源：http://gyf.daxiang520.top

char dst[32]; strcpy(dst, "hi");
来源：http://vew.hnqzz.top

[S05] C：字符串长度
来源：http://tbx.wangdashe.top

strlen(s)
来源：http://zmq.xinyue.icu

[S06] C：字符串比较
来源：http://tqh.xuetiantiany.cn

strcmp(a, b) == 0
来源：http://roc.nanxinkj.top

[S07] C：数组遍历求和
来源：http://qox.yuxming.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vwr.wangshuangyany.cn

[S08] C：动态内存分配与释放
来源：http://vet.ehwqpu.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://evd.zdbjq.cn

[S09] C：结构体定义与初始化
来源：http://xll.ehwqpu.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wwg.chenlongwang.top

[S10] C：指针与解引用
来源：http://ybp.havefunace.top

int *p = &a;  *p = 5;
来源：http://xgi.52xcode.cn

[S11] C：逐行读文件
来源：http://ggp.tarul.cn

FILE *f = fopen("a.txt", "r");
来源：http://rvj.fengsongda.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://cfm.sjlbkw.cn

fclose(f);
来源：http://zkq.zycfv.cn

[S12] C：写文件
来源：http://jdy.fktsv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ehs.jqgufenzy.top

[S13] C：宏定义
来源：http://ouy.ehwqpu.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gfs.hnxiangtu.top

[S14] C：枚举
来源：http://odv.bjfxy.top

enum Color { RED, GREEN, BLUE };
来源：http://bmc.shangyingyoupin.top

[S15] C：类型转换
来源：http://vss.mhx1999.top

(double) a / b
来源：http://wkv.hammf.cn

[S16] C：位操作置位
来源：http://lwr.tianlin.xyz

x |= (1 << 3);
来源：http://eku.iojbl.cn

[S17] C：安全拼接字符串
来源：http://aet.xylfe.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aek.yfazqb.com

[S18] C：命令行参数
来源：http://gxp.9152youxi.cn


<!-- 参考信息 -->