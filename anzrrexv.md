代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kjr.dianchejie.cn

[Q50] 批量更新
来源：http://djx.52xcode.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pzf.hammf.cn

[Q51] 用子查询更新
来源：http://ymb.zhongyouzk.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zzy.guannengcc.top

[Q52] 删除指定行
来源：http://jln.cucudq.cn

DELETE FROM users WHERE id = 10;
来源：http://cbi.cqqwz.cn

[Q53] 按条件删除
来源：http://suw.bjfxy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yzm.hfpthk.cn

[Q54] 清空表
来源：http://nfq.zhiwuduotai.top

TRUNCATE TABLE logs;
来源：http://qpy.smart0.xyz

[Q55] 排名（并列占位）
来源：http://dse.hnqzz.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vda.fzhhl.top

[Q56] 密集排名（并列不占位）
来源：http://ire.sufxvd.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pje.zdqjudy.top

[Q57] 行号
来源：http://buh.yueranfly.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nbj.xylfe.cn

[Q58] 累计求和
来源：http://qym.zhixingplan.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bcc.jinqigufen.top

[Q59] 分组内累计
来源：http://wdd.ydjk.org.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nwq.zhaomingkeji.xyz

[Q60] 取上一行 / 下一行
来源：http://dds.smart0.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rxx.sweek.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://osy.jinghuilouyu.cn

[Q61] 移动平均
来源：http://lnz.wangdashe.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bbg.jinqigfzy.top

[Q62] 分组占比
来源：http://vrp.ppjwa.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dxe.ivvv.top

[Q63] 开启事务
来源：http://cpi.hammf.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ieu.pycfn.com

[Q64] 提交事务
来源：http://tif.iojbl.cn

COMMIT;
来源：http://mor.wangshuangyany.cn

[Q65] 回滚事务
来源：http://bcr.nanxuanxn.top

ROLLBACK;
来源：http://rnu.316326.xyz

[Q66] 行锁查询
来源：http://cko.yuanzhike.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nmn.9152youxi.cn

[Q67] 设置隔离级别
来源：http://kkp.cashguo.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jys.shuidangran.top

[Q68] 保存点
来源：http://ois.ydjk.org.cn

SAVEPOINT sp1;
来源：http://lfw.hesvh.cn

ROLLBACK TO sp1;
来源：http://ckh.uphjek.com

[Q69] 查看执行计划
来源：http://bes.smart0.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hmk.cdnleiting.top

[Q70] 更新统计信息
来源：http://rnf.birdmap.top

ANALYZE TABLE users;
来源：http://eny.gotoacloud.top

[Q71] 查看建表语句
来源：http://nmy.hongshengwenyu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eqx.zhoulong.xyz

[Q72] 查看索引
来源：http://zhr.yuxming.cn

SHOW INDEX FROM users;
来源：http://flp.jinghuilouyu.cn

[Q73] 查看表状态
来源：http://kkq.jlsjyb.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jvg.jinqigufen.top

[Q74] 强制使用索引
来源：http://aqd.feifeiyinyue.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qqv.bjfxy.top

[Q75] 日期格式化
来源：http://ozi.daria6918.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ipz.ybcxt.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xsh.pengpengdd.cyou

[Q76] 按天统计
来源：http://pza.bjfxy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bto.xinyue.icu

[Q77] 时间加减
来源：http://wxj.cdnleiting.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://loy.jinqigufen.top

[Q78] 当前时间
来源：http://yob.hammf.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hfr.wangdashe.top

[Q79] 字符串拼接
来源：http://fjr.jyoumei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uoh.epnwcf.com

[Q80] 字符串截取
来源：http://sar.chenlongwang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lsp.ybcxt.top

[Q81] 字符串替换
来源：http://vod.jyoumei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://edv.jianghu66.top

[Q82] 字符长度与字节长度
来源：http://akd.hfpthk.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xtt.yvedp.cn

[Q83] 大小写转换
来源：http://myk.9152youxi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qbq.nwbrower.top

[Q84] 去除首尾空格
来源：http://rlb.sysykeji.top

SELECT TRIM(name) FROM users;
来源：http://rbd.hongshengwenyu.top

[Q85] 数值取整
来源：http://zcu.yuanzhike.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://oqp.yanxiufei.cn

[Q86] 读取 JSON 字段
来源：http://cts.jianghu66.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iyg.pengpengdd.cyou

[Q87] JSON 字段做条件
来源：http://lvc.hongshengwenyu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tzc.jyoumei.cn

[Q88] 行转列（条件聚合）
来源：http://vlt.smart0.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wfm.yvedp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tao.fanxiaobao.xyz

[Q89] 判断表是否存在
来源：http://tmz.cheryme.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jgu.yj20258.top

[Q90] 生成序号列
来源：http://bkt.nanxinkj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nxb.yanxiufei.cn

================================================================================
来源：http://aht.jinqigufen.top

R. Bash 专题
来源：http://ssk.aizwys.cn

================================================================================
来源：http://jww.9152youxi.cn

[R01] shebang 与严格模式
来源：http://pho.chenjidiqi.icu

#!/usr/bin/env bash
来源：http://wzw.yongpay.top

set -euo pipefail
来源：http://myl.pycfn.com

[R02] 变量赋值与使用
来源：http://nkm.yuanzhike.top

name="Tom"; echo "$name"
来源：http://yat.meibo888.top

[R03] 只读变量
来源：http://cmg.zdbjq.cn

readonly PI=3.14
来源：http://iiv.ehwqpu.com

[R04] 位置参数
来源：http://uxh.gotoacloud.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fps.shangyingyoupin.top

[R05] 参数默认值
来源：http://dio.zdqjudy.top

name="${1:-default}"
来源：http://nxi.yonumen.top

[R06] 判断命令是否存在
来源：http://fdt.pycfn.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jat.yj20258.top

[R07] if 判断文件
来源：http://htc.jyoumei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lcx.yuxming.cn

[R08] 数值比较
来源：http://kkz.dashuyun.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rdb.vehdjk.com

[R09] 字符串比较
来源：http://ato.tanke756.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://poe.yonumen.top

[R10] 正则匹配
来源：http://zlp.dashuyun.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://law.hcnkem.com

[R11] case 多分支
来源：http://wft.cdnleiting.top

case "$1" in
来源：http://edx.hnxiangtu.top

start) echo "启动" ;;
来源：http://rdd.tianlin.xyz

stop)  echo "停止" ;;
来源：http://xgb.ctjpmb.com

*)     echo "未知命令" ;;
来源：http://luu.gogol.net.cn

esac
来源：http://gwk.quarkkingdee.top

[R12] for 遍历文件
来源：http://wdi.sjlbkw.cn

for f in *.txt; do echo "$f"; done
来源：http://omm.shanyushiyangkeji.top

[R13] for 计数循环
来源：http://fwh.ybcxt.top

for i in {1..10}; do echo "$i"; done
来源：http://oqs.bjfxy.top

[R14] C 风格 for
来源：http://qhn.ctjpmb.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nmh.shzxlz.cn

[R15] while 逐行读文件
来源：http://rmr.sxryk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cyb.hesvh.cn

[R16] until 等待条件
来源：http://skl.kuanghao11.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://crz.smart0.xyz

[R17] 数组定义与取值
来源：http://icp.sufxvd.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mmj.pengpengdd.cyou

[R18] 遍历数组
来源：http://wxd.vehdjk.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zcu.jqgfzy.top

[R19] 数组长度
来源：http://ejh.xingfuxueyuan.xyz

echo "${#arr[@]}"
来源：http://gch.feifeiyinyue.top

[R20] 关联数组（字典）
来源：http://jxd.redwolf501.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://whs.wangdashe.top

[R21] 字符串长度
来源：http://wct.hfpthk.cn

echo "${#s}"
来源：http://rbp.hongshengwenyu.top

[R22] 截取子串
来源：http://mam.ybcxt.top

echo "${s:0:5}"
来源：http://nhu.52xcode.cn

[R23] 字符串替换
来源：http://dng.yj20258.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yys.epnwcf.com

[R24] 大小写转换
来源：http://jrl.vehdjk.com

echo "${s^^}"; echo "${s,,}"
来源：http://xzf.jianghu66.top

[R25] 去后缀 / 去前缀
来源：http://luh.jqgufenzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ntx.snrcjt.cn

[R26] 命令替换
来源：http://pht.jianghu66.top

now=$(date +%F); echo "$now"
来源：http://tta.pycfn.com

[R27] 算术展开
来源：http://koa.iojbl.cn

echo $((1 + 2 * 3))
来源：http://xrm.hcnkem.com

[R28] 浮点运算
来源：http://ikp.zdbjq.cn

echo "scale=2; 10/3" | bc
来源：http://ufi.jqgfzy.top

[R29] 定义函数
来源：http://yke.epnwcf.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://syu.pengpengdd.cyou

[R30] 函数返回状态码
来源：http://anf.pycfn.com

f() { return 0; }; f || echo "失败了"
来源：http://mkz.jinghuilouyu.cn

[R31] 局部变量
来源：http://tdm.jqgfzy.top

f() { local x=1; echo "$x"; }
来源：http://vxx.sysykeji.top

[R32] 参数个数校验
来源：http://zoe.havefunace.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yex.fengsongda.top

[R33] 捕获错误并提示行号
来源：http://gym.jqgufenzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bbr.fktsv.cn

[R34] 退出时清理
来源：http://nst.haohaochexian.top

trap 'rm -f "$tmp"' EXIT
来源：http://yco.nanxuanxn.top

[R35] 后台执行并等待
来源：http://tpi.shanyushiyangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://voa.ybcxt.top

[R36] 并发执行多个任务
来源：http://jox.hnxiangtu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tgn.shanyushiyangtech.top

[R37] 把输出赋给变量
来源：http://ldx.yueranfly.top

files=$(ls -1)
来源：http://uxb.quarkkingdee.top

[R38] 管道串联
来源：http://meh.zdqjudy.top

cat a.txt | grep -i error | wc -l
来源：http://qnp.meibo888.top

[R39] 重定向标准输出与错误
来源：http://vjo.jianghu66.top

cmd > out.log 2>&1
来源：http://sxs.hnqzz.top

[R40] 追加写日志
来源：http://drd.fengsongda.top

echo "log" >> out.log
来源：http://jhy.tianlin.xyz

[R41] 丢弃输出
来源：http://nwg.kuanghao11.cn

cmd >/dev/null 2>&1
来源：http://dri.xingfuxueyuan.xyz

[R42] 输入重定向
来源：http://pye.yueranfly.top

wc -l < a.txt
来源：http://pqs.xylfe.cn

[R43] 按名字查找文件
来源：http://vay.zhijiandao.cn

find . -name "*.log" -type f
来源：http://ekv.9152youxi.cn

[R44] 按修改时间查找
来源：http://gfc.iojbl.cn

find . -mtime -7 -type f
来源：http://jzj.havefunace.top

[R45] 批量删除
来源：http://pku.aibaodan.cn

find . -name "*.tmp" -delete
来源：http://bxb.bjfxy.top

[R46] 递归替换文件内容
来源：http://zfg.shangyingyoupin.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bbp.xinyue.icu

[R47] sed 单行替换
来源：http://hed.sufxvd.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hml.chenjidiqi.icu

[R48] awk 取指定列
来源：http://hac.yueranfly.top

awk '{print $1, $3}' a.txt
来源：http://dpf.gogol.net.cn

[R49] awk 带条件
来源：http://rsh.jinghuilouyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://icc.sufxvd.cn

[R50] awk 求和
来源：http://yml.jiagoushi.top

awk '{s += $2} END {print s}' a.txt
来源：http://som.smart0.xyz

[R51] 排序去重取前几
来源：http://spw.shanyushiyangtech.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ish.guowangkeji.top

[R52] 统计行数
来源：http://prn.jinghuilouyu.cn

wc -l a.txt
来源：http://bpw.uphjek.com

[R53] 查看文件头与实时尾
来源：http://phc.jqgufenzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gmt.vehdjk.com

[R54] 比较两个文件
来源：http://uib.guowangkeji.top

diff a.txt b.txt
来源：http://ytt.meibo888.top

[R55] 压缩与解压
来源：http://szk.shanyushiyangtech.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nhx.gogol.net.cn

[R56] 远程拷贝
来源：http://qkk.dianchejie.cn

scp file user@host:/path/
来源：http://mnl.0kj1m.cn

[R57] 远程执行命令
来源：http://xwy.sufxvd.cn

ssh user@host 'uptime'
来源：http://rzf.sweek.top

[R58] 下载文件
来源：http://rqj.gotoacloud.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://viz.mhx1999.top

[R59] 发 POST JSON
来源：http://rrc.zhongyouzk.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qhd.hnxiangtu.top

[R60] 只看 HTTP 状态码
来源：http://nmn.fengsongda.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xvu.gotoacloud.top

[R61] 磁盘占用
来源：http://tnk.shuidangran.top

df -h;  du -sh *
来源：http://nyq.meibo888.top

[R62] 找最占空间的文件
来源：http://kul.mhx1999.top

du -ah . | sort -rh | head -10
来源：http://gri.fanxiaobao.xyz

[R63] 内存与进程
来源：http://gum.chenlongwang.top

free -h;  ps aux | grep nginx
来源：http://jrj.vqdsnc.cn

[R64] 结束进程
来源：http://rrr.aizwys.cn

kill -9 $(pgrep -f app.py)
来源：http://cvk.yuanzhike.top

[R65] 查看端口占用
来源：http://zbc.meibo888.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nno.kuanghao11.cn

[R66] 定时任务
来源：http://lvs.quarkkingdee.top

crontab -e;  crontab -l
来源：http://qcz.hnxiangtu.top

[R67] 生成随机十六进制串
来源：http://hmn.iojbl.cn

openssl rand -hex 16
来源：http://pyd.shuidangran.top

[R68] 计算文件校验值
来源：http://nue.cdnleiting.top

sha256sum a.txt;  md5sum a.txt
来源：http://mqy.yanxiufei.cn

[R69] 生成随机密码
来源：http://qyf.jiagoushi.top

head -c 16 /dev/urandom | base64
来源：http://kqu.0kj1m.cn

[R70] 时间戳与互转
来源：http://jym.mhx1999.top

date +%s;  date -d @1700000000
来源：http://anr.zycfv.cn

[R71] 日期格式化
来源：http://lud.hcnkem.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://quj.yonumen.top

[R72] 等待端口就绪
来源：http://hxm.chenzaomai.com

until nc -z localhost 3306; do sleep 1; done
来源：http://qql.pengpengdd.cyou

[R73] 分割大日志
来源：http://jwz.hcnkem.com

split -l 1000 big.log part_
来源：http://dvk.yonumen.top

[R74] 批量重命名
来源：http://wmt.tian-w.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://anv.nanxinkj.top

[R75] 导出环境变量
来源：http://gpx.jqgfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://cpq.ydjk.org.cn

[R76] 使用临时文件
来源：http://nzq.9152youxi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oja.zhongyouzk.top

[R77] 读取用户输入
来源：http://yor.ywan-chungtsiang.top

read -rp "请输入: " ans
来源：http://rte.gaohongyu789.top

[R78] 交互式菜单
来源：http://xju.ehwqpu.com

select opt in a b c; do echo "$opt"; break; done
来源：http://vqt.9152youxi.cn

[R79] 解析命令行选项
来源：http://tte.bjfxy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kwn.jinyuanbaomall.cn

[R80] 查看脚本执行耗时
来源：http://gpz.yuxming.cn

time ./run.sh
来源：http://mwd.wangdashe.top

================================================================================
来源：http://ham.ppjwa.cn

S. C / C++ 专题
来源：http://zwc.c1oappe.top

================================================================================
来源：http://dql.smart0.xyz

[S01] C：Hello World
来源：http://ptd.fanxiaobao.xyz

#include <stdio.h>
来源：http://whm.tianlin.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://blu.yvedp.cn

[S02] C：变量与格式化输出
来源：http://cnm.zhengqikj.top

int a = 10; printf("%d\n", a);
来源：http://hsf.uphjek.com

[S03] C：读入整数
来源：http://nly.yj20258.top

int x; scanf("%d", &x);
来源：http://mgy.tianlin.xyz

[S04] C：字符串复制
来源：http://upj.snrcjt.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ilr.daria6918.cn

[S05] C：字符串长度
来源：http://ars.52xcode.cn

strlen(s)
来源：http://zvv.fehbvm.com

[S06] C：字符串比较
来源：http://trp.haohaochexian.top

strcmp(a, b) == 0
来源：http://tbd.xuetiantiany.cn

[S07] C：数组遍历求和
来源：http://qsg.meibo888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mpj.uphjek.com

[S08] C：动态内存分配与释放
来源：http://yzw.cheryme.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mqe.birdmap.top

[S09] C：结构体定义与初始化
来源：http://wmf.ivvv.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mmy.svipenyu.cn

[S10] C：指针与解引用
来源：http://ytx.nanxuanxn.top

int *p = &a;  *p = 5;
来源：http://wap.jqgufenzy.top

[S11] C：逐行读文件
来源：http://qpg.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "r");
来源：http://ydu.mhx1999.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ftn.ybcxt.top

fclose(f);
来源：http://tnk.cashguo.top

[S12] C：写文件
来源：http://qsb.52xcode.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qwa.zhiwuduotai.top

[S13] C：宏定义
来源：http://oog.cdnleiting.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qgl.c1oappe.top

[S14] C：枚举
来源：http://wdu.kuanghao11.cn

enum Color { RED, GREEN, BLUE };
来源：http://vkc.fanxiaobao.xyz

[S15] C：类型转换
来源：http://xzz.hongshengwenyu.top

(double) a / b
来源：http://nlu.yj20258888.top

[S16] C：位操作置位
来源：http://wrw.jinqigfzy.top

x |= (1 << 3);
来源：http://hue.hnqzz.top

[S17] C：安全拼接字符串
来源：http://nno.shzxlz.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pdb.ctjpmb.com

[S18] C：命令行参数
来源：http://vwn.ybcxt.top

int main(int argc, char **argv)
来源：http://mdg.wangshuangyany.cn

[S19] C：快速排序
来源：http://cio.havefunace.top

qsort(a, n, sizeof(int), cmp);
来源：http://boz.vqdsnc.cn

[S20] C：二分查找
来源：http://nsn.xuanzx.com


<!-- 参考信息 -->