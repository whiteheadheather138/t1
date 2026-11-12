代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cdj.yueranfly.top

[Q50] 批量更新
来源：http://mcy.aibaodan.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zhz.jiagoushi.top

[Q51] 用子查询更新
来源：http://grj.hnqzz.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hrf.fehbvm.com

[Q52] 删除指定行
来源：http://qnp.yvedp.cn

DELETE FROM users WHERE id = 10;
来源：http://ncr.xziqi.cn

[Q53] 按条件删除
来源：http://yhp.hnqzz.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hez.daxiang520.top

[Q54] 清空表
来源：http://qtx.guannengcc.top

TRUNCATE TABLE logs;
来源：http://rdh.aizwys.cn

[Q55] 排名（并列占位）
来源：http://gqe.cdnleiting.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://drh.iojbl.cn

[Q56] 密集排名（并列不占位）
来源：http://ssc.sysykeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gvk.zdqjudy.top

[Q57] 行号
来源：http://pmo.zhiwuduotai.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ihj.shangyingyoupin.top

[Q58] 累计求和
来源：http://pyr.aibaodan.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zhf.sysykeji.top

[Q59] 分组内累计
来源：http://jwr.quarkkingdee.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nov.zdqjudy.top

[Q60] 取上一行 / 下一行
来源：http://pxs.quarkkingdee.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oty.yueranfly.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fil.shzxlz.cn

[Q61] 移动平均
来源：http://ybr.meibo888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ryc.sysykeji.top

[Q62] 分组占比
来源：http://hkq.xinyue.icu

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://iao.jinghuilouyu.cn

[Q63] 开启事务
来源：http://gae.zhijiandao.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cfx.yj20258.top

[Q64] 提交事务
来源：http://ugd.316326.xyz

COMMIT;
来源：http://lqk.tanke756.top

[Q65] 回滚事务
来源：http://skd.yanxiufei.cn

ROLLBACK;
来源：http://jrg.9152youxi.cn

[Q66] 行锁查询
来源：http://weq.uphjek.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lyl.gotoacloud.top

[Q67] 设置隔离级别
来源：http://ktu.ydzc1.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jla.ywan-chungtsiang.top

[Q68] 保存点
来源：http://kvi.jiagoushi.top

SAVEPOINT sp1;
来源：http://dig.yj20258.top

ROLLBACK TO sp1;
来源：http://gyf.hysaishi.cn

[Q69] 查看执行计划
来源：http://yyn.fehbvm.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://grx.jinyuanbaomall.cn

[Q70] 更新统计信息
来源：http://pux.quarkkingdee.top

ANALYZE TABLE users;
来源：http://ykv.meibo888.top

[Q71] 查看建表语句
来源：http://byp.dianchejie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xgj.zdbjq.cn

[Q72] 查看索引
来源：http://qpm.guannengcc.top

SHOW INDEX FROM users;
来源：http://bgh.bbcook.cn

[Q73] 查看表状态
来源：http://grp.yfazqb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://ueo.chenlongwang.top

[Q74] 强制使用索引
来源：http://ttm.jyoumei.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tjy.cucudq.cn

[Q75] 日期格式化
来源：http://evl.aizwys.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gpg.gotoacloud.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mld.hnxiangtu.top

[Q76] 按天统计
来源：http://mdl.sjlbkw.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fuq.snrcjt.cn

[Q77] 时间加减
来源：http://kpr.bjfxy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hmh.nanxuanxn.top

[Q78] 当前时间
来源：http://cyj.sufxvd.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xhb.shangyingyoupin.top

[Q79] 字符串拼接
来源：http://rlw.mhx1999.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iml.tian-w.cn

[Q80] 字符串截取
来源：http://tji.yongpay.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rye.zhijiandao.cn

[Q81] 字符串替换
来源：http://qxp.yanxiufei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yol.hongshengwenyu.top

[Q82] 字符长度与字节长度
来源：http://hmy.daria6918.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ila.fzhhl.top

[Q83] 大小写转换
来源：http://blw.aizwys.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nhd.52xcode.cn

[Q84] 去除首尾空格
来源：http://msm.tanke756.top

SELECT TRIM(name) FROM users;
来源：http://yhz.gotoacloud.top

[Q85] 数值取整
来源：http://aau.cashguo.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mfz.yvedp.cn

[Q86] 读取 JSON 字段
来源：http://mkb.xziqi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lfp.cucudq.cn

[Q87] JSON 字段做条件
来源：http://sky.epnwcf.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iwv.yj20258.top

[Q88] 行转列（条件聚合）
来源：http://pdp.zhijiandao.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pjx.meibo888.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tvt.daxiang520.top

[Q89] 判断表是否存在
来源：http://ytq.feifeiyinyue.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dua.tarul.cn

[Q90] 生成序号列
来源：http://pcf.ivvv.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rfa.hnqzz.top

================================================================================
来源：http://yfh.aibaodan.cn

R. Bash 专题
来源：http://sqi.shanyushiyangtech.top

================================================================================
来源：http://szy.gogol.net.cn

[R01] shebang 与严格模式
来源：http://juw.ivvv.top

#!/usr/bin/env bash
来源：http://ite.aizwys.cn

set -euo pipefail
来源：http://qgi.daria6918.cn

[R02] 变量赋值与使用
来源：http://nur.vqdsnc.cn

name="Tom"; echo "$name"
来源：http://uai.gzhubu.top

[R03] 只读变量
来源：http://jqj.chenlongwang.top

readonly PI=3.14
来源：http://pqg.jinqigufen.top

[R04] 位置参数
来源：http://ikq.cheryme.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ora.redwolf501.top

[R05] 参数默认值
来源：http://pzp.hongshengwenyu.top

name="${1:-default}"
来源：http://jdd.jianghu66.top

[R06] 判断命令是否存在
来源：http://zsj.cdnleiting.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zsh.ydzc1.top

[R07] if 判断文件
来源：http://lhv.nanxuanxn.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qxw.dianchejie.cn

[R08] 数值比较
来源：http://biw.fktsv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zcz.nanxinkj.top

[R09] 字符串比较
来源：http://hec.guowangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cow.cashguo.top

[R10] 正则匹配
来源：http://uqj.shanyushiyangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dxw.dashuyun.cn

[R11] case 多分支
来源：http://byp.ctjpmb.com

case "$1" in
来源：http://hcw.fzhhl.top

start) echo "启动" ;;
来源：http://amu.smart0.xyz

stop)  echo "停止" ;;
来源：http://esw.redwolf501.top

*)     echo "未知命令" ;;
来源：http://jmj.xinyue.icu

esac
来源：http://hie.9152youxi.cn

[R12] for 遍历文件
来源：http://wvt.hywenlv.cn

for f in *.txt; do echo "$f"; done
来源：http://nlk.chenzaomai.com

[R13] for 计数循环
来源：http://czg.yuxming.cn

for i in {1..10}; do echo "$i"; done
来源：http://mzt.yj20258888.top

[R14] C 风格 for
来源：http://sjq.dashuyun.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://obj.jinyuanbaomall.cn

[R15] while 逐行读文件
来源：http://irz.jqgufenzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tvo.hysaishi.cn

[R16] until 等待条件
来源：http://pdg.shanyushiyangtech.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ljg.fengsongda.top

[R17] 数组定义与取值
来源：http://cle.0kj1m.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ama.yuanzhike.top

[R18] 遍历数组
来源：http://tbo.hammf.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xea.ivvv.top

[R19] 数组长度
来源：http://wev.jinyuanbaomall.cn

echo "${#arr[@]}"
来源：http://pbr.birdmap.top

[R20] 关联数组（字典）
来源：http://fep.yfazqb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://czh.nanxuanxn.top

[R21] 字符串长度
来源：http://rat.xziqi.cn

echo "${#s}"
来源：http://yrd.pycfn.com

[R22] 截取子串
来源：http://jwi.fzhhl.top

echo "${s:0:5}"
来源：http://eay.9152youxi.cn

[R23] 字符串替换
来源：http://oim.jinqigfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eip.kuanghao11.cn

[R24] 大小写转换
来源：http://lvy.zhongyouzk.top

echo "${s^^}"; echo "${s,,}"
来源：http://uzj.316326.xyz

[R25] 去后缀 / 去前缀
来源：http://lkm.kuanghao11.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cnf.andypj.xyz

[R26] 命令替换
来源：http://bqe.xuetiantiany.cn

now=$(date +%F); echo "$now"
来源：http://zsw.c1oappe.top

[R27] 算术展开
来源：http://axj.haohaochexian.top

echo $((1 + 2 * 3))
来源：http://jdr.vqdsnc.cn

[R28] 浮点运算
来源：http://czu.yfazqb.com

echo "scale=2; 10/3" | bc
来源：http://dvr.meibo888.top

[R29] 定义函数
来源：http://cwm.nanxuanxn.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bkg.ydjk.org.cn

[R30] 函数返回状态码
来源：http://ziu.hongshengwenyu.top

f() { return 0; }; f || echo "失败了"
来源：http://etj.fzhhl.top

[R31] 局部变量
来源：http://fgc.yfazqb.com

f() { local x=1; echo "$x"; }
来源：http://ako.yvedp.cn

[R32] 参数个数校验
来源：http://dwx.shangyingyoupin.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mqp.9152youxi.cn

[R33] 捕获错误并提示行号
来源：http://saa.jinyuanbaomall.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uhc.ehwqpu.com

[R34] 退出时清理
来源：http://ufk.shzxlz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nkl.yongpay.top

[R35] 后台执行并等待
来源：http://ebx.tianlin.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://lrm.ydzc1.top

[R36] 并发执行多个任务
来源：http://zfh.sufxvd.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jaj.fzhhl.top

[R37] 把输出赋给变量
来源：http://itf.sxryk.cn

files=$(ls -1)
来源：http://mow.pengpengdd.cyou

[R38] 管道串联
来源：http://gqf.sjlbkw.cn

cat a.txt | grep -i error | wc -l
来源：http://sil.ybcxt.top

[R39] 重定向标准输出与错误
来源：http://lcp.bbcook.cn

cmd > out.log 2>&1
来源：http://gpm.yueranfly.top

[R40] 追加写日志
来源：http://eei.redwolf501.top

echo "log" >> out.log
来源：http://vpg.shanyushiyangtech.top

[R41] 丢弃输出
来源：http://kxd.hammf.cn

cmd >/dev/null 2>&1
来源：http://luo.kuanghao11.cn

[R42] 输入重定向
来源：http://gkd.yonumen.top

wc -l < a.txt
来源：http://rxr.sjlbkw.cn

[R43] 按名字查找文件
来源：http://xkf.ydjk.org.cn

find . -name "*.log" -type f
来源：http://xqe.dianchejie.cn

[R44] 按修改时间查找
来源：http://vqj.nanxuanxn.top

find . -mtime -7 -type f
来源：http://flp.iojbl.cn

[R45] 批量删除
来源：http://ioo.shanyushiyangkeji.top

find . -name "*.tmp" -delete
来源：http://miu.zhiwuduotai.top

[R46] 递归替换文件内容
来源：http://gsb.gzhubu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dic.shanyushiyangtech.top

[R47] sed 单行替换
来源：http://qbb.gaohongyu789.top

sed -i 's/foo/bar/g' a.txt
来源：http://mpq.vehdjk.com

[R48] awk 取指定列
来源：http://ziw.zhiwuduotai.top

awk '{print $1, $3}' a.txt
来源：http://bpg.guowangkeji.top

[R49] awk 带条件
来源：http://lby.ybcxt.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wpr.sysykeji.top

[R50] awk 求和
来源：http://hyd.daxiang520.top

awk '{s += $2} END {print s}' a.txt
来源：http://dtd.yj20258.top

[R51] 排序去重取前几
来源：http://dve.jqgfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://isk.fzhhl.top

[R52] 统计行数
来源：http://aeo.9152youxi.cn

wc -l a.txt
来源：http://qws.sweek.top

[R53] 查看文件头与实时尾
来源：http://nsk.xylfe.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iaj.xziqi.cn

[R54] 比较两个文件
来源：http://rcb.epnwcf.com

diff a.txt b.txt
来源：http://cig.chenlongwang.top

[R55] 压缩与解压
来源：http://zpk.xingfuxueyuan.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mbi.uphjek.com

[R56] 远程拷贝
来源：http://blk.hfpthk.cn

scp file user@host:/path/
来源：http://kft.redwolf501.top

[R57] 远程执行命令
来源：http://fnq.yj202588.top

ssh user@host 'uptime'
来源：http://kjp.shuidangran.top

[R58] 下载文件
来源：http://ptv.yongpay.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ggi.vqdsnc.cn

[R59] 发 POST JSON
来源：http://zoa.uphjek.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uvu.pycfn.com

[R60] 只看 HTTP 状态码
来源：http://otp.fehbvm.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ytg.zhengqikj.top

[R61] 磁盘占用
来源：http://ahy.chenzaomai.com

df -h;  du -sh *
来源：http://svq.ivvv.top

[R62] 找最占空间的文件
来源：http://nun.jiagoushi.top

du -ah . | sort -rh | head -10
来源：http://tfz.sweek.top

[R63] 内存与进程
来源：http://spt.cashguo.top

free -h;  ps aux | grep nginx
来源：http://ejd.zhongyouzk.top

[R64] 结束进程
来源：http://krq.chenlongwang.top

kill -9 $(pgrep -f app.py)
来源：http://ipn.yongpay.top

[R65] 查看端口占用
来源：http://mry.snrcjt.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vhp.fanxiaobao.xyz

[R66] 定时任务
来源：http://bnk.quarkkingdee.top

crontab -e;  crontab -l
来源：http://tnk.zdbjq.cn

[R67] 生成随机十六进制串
来源：http://dvj.gogol.net.cn

openssl rand -hex 16
来源：http://ucq.sufxvd.cn

[R68] 计算文件校验值
来源：http://bkl.fengsongda.top

sha256sum a.txt;  md5sum a.txt
来源：http://tev.ydjk.org.cn

[R69] 生成随机密码
来源：http://pov.hywenlv.cn

head -c 16 /dev/urandom | base64
来源：http://gmo.aizwys.cn

[R70] 时间戳与互转
来源：http://tpr.ehwqpu.com

date +%s;  date -d @1700000000
来源：http://rdt.xziqi.cn

[R71] 日期格式化
来源：http://efz.daria6918.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gtk.gogol.net.cn

[R72] 等待端口就绪
来源：http://uay.tarul.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xuq.dashuyun.cn

[R73] 分割大日志
来源：http://nof.hongshengwenyu.top

split -l 1000 big.log part_
来源：http://zkr.redwolf501.top

[R74] 批量重命名
来源：http://wud.pengpengdd.cyou

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fsn.yj20258.top

[R75] 导出环境变量
来源：http://ggk.ctjpmb.com

export PATH="$HOME/bin:$PATH"
来源：http://bcy.kuanghao11.cn

[R76] 使用临时文件
来源：http://ayo.sjlbkw.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://amv.gotoacloud.top

[R77] 读取用户输入
来源：http://lsl.ctjpmb.com

read -rp "请输入: " ans
来源：http://ghd.hywenlv.cn

[R78] 交互式菜单
来源：http://phx.yj20258888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://due.fengsongda.top

[R79] 解析命令行选项
来源：http://nlm.aizwys.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ohv.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://fai.zhongyouzk.top

time ./run.sh
来源：http://xlm.vehdjk.com

================================================================================
来源：http://kql.dianchejie.cn

S. C / C++ 专题
来源：http://aqs.shanyushiyangtech.top

================================================================================
来源：http://tvu.fengsongda.top

[S01] C：Hello World
来源：http://vsw.iojbl.cn

#include <stdio.h>
来源：http://psq.bjfxy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://yuq.nanxinkj.top

[S02] C：变量与格式化输出
来源：http://diy.yuxming.cn

int a = 10; printf("%d\n", a);
来源：http://blh.pengpengdd.cyou

[S03] C：读入整数
来源：http://edm.fengsongda.top

int x; scanf("%d", &x);
来源：http://xce.jinghuilouyu.cn

[S04] C：字符串复制
来源：http://mdn.ivvv.top

char dst[32]; strcpy(dst, "hi");
来源：http://jch.birdmap.top

[S05] C：字符串长度
来源：http://nal.yueranfly.top

strlen(s)
来源：http://rgs.yj202588.top

[S06] C：字符串比较
来源：http://tab.guannengcc.top

strcmp(a, b) == 0
来源：http://jjs.dianchejie.cn

[S07] C：数组遍历求和
来源：http://xde.meibo888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eep.zhoulong.xyz

[S08] C：动态内存分配与释放
来源：http://ctb.fanxiaobao.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://aol.hfpthk.cn

[S09] C：结构体定义与初始化
来源：http://ogm.0kj1m.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mvn.aibaodan.cn

[S10] C：指针与解引用
来源：http://uet.aizwys.cn

int *p = &a;  *p = 5;
来源：http://obb.fktsv.cn

[S11] C：逐行读文件
来源：http://bom.redwolf501.top

FILE *f = fopen("a.txt", "r");
来源：http://pto.yueranfly.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://gak.aibaodan.cn

fclose(f);
来源：http://kfq.feifeiyinyue.top

[S12] C：写文件
来源：http://zhr.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dyi.sweek.top

[S13] C：宏定义
来源：http://huf.haohaochexian.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jac.andypj.xyz

[S14] C：枚举
来源：http://kup.fehbvm.com

enum Color { RED, GREEN, BLUE };
来源：http://hbe.shanyushiyangkeji.top

[S15] C：类型转换
来源：http://ver.sjlbkw.cn

(double) a / b
来源：http://gmk.cashguo.top

[S16] C：位操作置位
来源：http://myn.aizwys.cn

x |= (1 << 3);
来源：http://apu.hnqzz.top

[S17] C：安全拼接字符串
来源：http://yfl.yangfankeji.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yob.hcnkem.com

[S18] C：命令行参数
来源：http://jan.ehwqpu.com

int main(int argc, char **argv)
来源：http://itn.ppjwa.cn

[S19] C：快速排序
来源：http://qwo.jinqigfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://wqk.kuanghao11.cn

[S20] C：二分查找
来源：http://aap.fktsv.cn


<!-- 参考信息 -->