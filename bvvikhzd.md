代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://myg.ydzc1.top

[Q52] 删除指定行
来源：http://ces.zhiwuduotai.top

DELETE FROM users WHERE id = 10;
来源：http://eek.zhoulong.xyz

[Q53] 按条件删除
来源：http://xvs.jinqigfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://skp.xuetiantiany.cn

[Q54] 清空表
来源：http://bki.fehbvm.com

TRUNCATE TABLE logs;
来源：http://hkv.tanke756.top

[Q55] 排名（并列占位）
来源：http://ety.yfazqb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mzv.mhx1999.top

[Q56] 密集排名（并列不占位）
来源：http://zpo.zhengqikj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jqq.haohaochexian.top

[Q57] 行号
来源：http://lox.xuetiantiany.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kgh.svipenyu.cn

[Q58] 累计求和
来源：http://rjq.mhx1999.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bps.uphjek.com

[Q59] 分组内累计
来源：http://ejw.guannengcc.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://auk.mhx1999.top

[Q60] 取上一行 / 下一行
来源：http://gal.hesvh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jzp.vehdjk.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://khu.jyoumei.cn

[Q61] 移动平均
来源：http://wnx.wangdashe.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xin.316326.xyz

[Q62] 分组占比
来源：http://bou.shuidangran.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hpo.9152youxi.cn

[Q63] 开启事务
来源：http://oam.pycfn.com

START TRANSACTION;                -- 或 BEGIN
来源：http://yry.jinyuanbaomall.cn

[Q64] 提交事务
来源：http://csc.tianlin.xyz

COMMIT;
来源：http://zip.cheryme.top

[Q65] 回滚事务
来源：http://apg.ppjwa.cn

ROLLBACK;
来源：http://nsr.gogol.net.cn

[Q66] 行锁查询
来源：http://nhh.52xcode.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oey.bbcook.cn

[Q67] 设置隔离级别
来源：http://bzu.tianlin.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xey.hysaishi.cn

[Q68] 保存点
来源：http://apc.yanxiufei.cn

SAVEPOINT sp1;
来源：http://ahu.gotoacloud.top

ROLLBACK TO sp1;
来源：http://ama.yj20258.top

[Q69] 查看执行计划
来源：http://xko.9152youxi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ggg.cheryme.top

[Q70] 更新统计信息
来源：http://ive.shanyushiyangkeji.top

ANALYZE TABLE users;
来源：http://dyg.uphjek.com

[Q71] 查看建表语句
来源：http://jvi.yj202588.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jpw.vqdsnc.cn

[Q72] 查看索引
来源：http://aev.ybcxt.top

SHOW INDEX FROM users;
来源：http://nze.gogol.net.cn

[Q73] 查看表状态
来源：http://fyz.aizwys.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cbs.zdqjudy.top

[Q74] 强制使用索引
来源：http://xoq.yuanzhike.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uua.fanxiaobao.xyz

[Q75] 日期格式化
来源：http://job.vqdsnc.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://glt.9152youxi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fha.ydzc1.top

[Q76] 按天统计
来源：http://jgc.yueranfly.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ddj.chenlongwang.top

[Q77] 时间加减
来源：http://sxs.wangdashe.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://afm.jiagoushi.top

[Q78] 当前时间
来源：http://ihk.jinqigfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://flc.chenjidiqi.icu

[Q79] 字符串拼接
来源：http://jtc.zhiwuduotai.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lcg.jinghuilouyu.cn

[Q80] 字符串截取
来源：http://mvp.fzhhl.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lub.zhaomingkeji.xyz

[Q81] 字符串替换
来源：http://spm.jiagoushi.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zhf.xinyue.icu

[Q82] 字符长度与字节长度
来源：http://dhm.andypj.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://chm.andypj.xyz

[Q83] 大小写转换
来源：http://qmc.ybcxt.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cjh.pengpengdd.cyou

[Q84] 去除首尾空格
来源：http://zsy.yj20258888.top

SELECT TRIM(name) FROM users;
来源：http://ndr.jyoumei.cn

[Q85] 数值取整
来源：http://apm.aizwys.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jdi.svipenyu.cn

[Q86] 读取 JSON 字段
来源：http://hig.jinqigufen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ahx.tian-w.cn

[Q87] JSON 字段做条件
来源：http://swx.dianchejie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tuj.svipenyu.cn

[Q88] 行转列（条件聚合）
来源：http://vor.meibo888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cxj.52xcode.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ywl.hongshengwenyu.top

[Q89] 判断表是否存在
来源：http://mgu.havefunace.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rqd.iojbl.cn

[Q90] 生成序号列
来源：http://ruw.xylfe.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cfa.ctjpmb.com

================================================================================
来源：http://mhp.gzhubu.top

R. Bash 专题
来源：http://zpp.zhengqikj.top

================================================================================
来源：http://hlz.hnqzz.top

[R01] shebang 与严格模式
来源：http://kad.shanyushiyangkeji.top

#!/usr/bin/env bash
来源：http://wnf.ppjwa.cn

set -euo pipefail
来源：http://lnx.shanyushiyangtech.top

[R02] 变量赋值与使用
来源：http://zym.jianghu66.top

name="Tom"; echo "$name"
来源：http://jhk.0kj1m.cn

[R03] 只读变量
来源：http://dkn.pycfn.com

readonly PI=3.14
来源：http://ojk.redwolf501.top

[R04] 位置参数
来源：http://ouw.sxryk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xgt.jiagoushi.top

[R05] 参数默认值
来源：http://pia.hnqzz.top

name="${1:-default}"
来源：http://ego.jinqigfzy.top

[R06] 判断命令是否存在
来源：http://vwa.9152youxi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ogt.fehbvm.com

[R07] if 判断文件
来源：http://usd.daria6918.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lfo.yanxiufei.cn

[R08] 数值比较
来源：http://btk.jiagoushi.top

if (( a > b )); then echo "a 更大"; fi
来源：http://lju.yuxming.cn

[R09] 字符串比较
来源：http://ukg.zhaomingkeji.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kst.chenjidiqi.icu

[R10] 正则匹配
来源：http://lwq.hesvh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kqd.zhixingplan.top

[R11] case 多分支
来源：http://tqr.haohaochexian.top

case "$1" in
来源：http://aic.9152youxi.cn

start) echo "启动" ;;
来源：http://san.chenlongwang.top

stop)  echo "停止" ;;
来源：http://tji.hywenlv.cn

*)     echo "未知命令" ;;
来源：http://gnr.mhx1999.top

esac
来源：http://xqf.jqgfzy.top

[R12] for 遍历文件
来源：http://viv.gaohongyu789.top

for f in *.txt; do echo "$f"; done
来源：http://zuq.yj20258.top

[R13] for 计数循环
来源：http://zay.daria6918.cn

for i in {1..10}; do echo "$i"; done
来源：http://grw.ctjpmb.com

[R14] C 风格 for
来源：http://zng.wangshuangyany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xze.jinghuilouyu.cn

[R15] while 逐行读文件
来源：http://vbh.zhoulong.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bsv.tianlin.xyz

[R16] until 等待条件
来源：http://epw.yj20258888.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wzi.cdnleiting.top

[R17] 数组定义与取值
来源：http://bbu.hnqzz.top

arr=(a b c); echo "${arr[0]}"
来源：http://eao.wangdashe.top

[R18] 遍历数组
来源：http://pqe.sufxvd.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bhs.xingfuxueyuan.xyz

[R19] 数组长度
来源：http://czt.yj20258888.top

echo "${#arr[@]}"
来源：http://jgd.ydjk.org.cn

[R20] 关联数组（字典）
来源：http://sqn.pycfn.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://das.hongshengwenyu.top

[R21] 字符串长度
来源：http://gzz.316326.xyz

echo "${#s}"
来源：http://etc.andypj.xyz

[R22] 截取子串
来源：http://lmd.fengsongda.top

echo "${s:0:5}"
来源：http://xtm.vqdsnc.cn

[R23] 字符串替换
来源：http://lyt.vqdsnc.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://etn.yonumen.top

[R24] 大小写转换
来源：http://eed.wangshuangyany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mgj.ehwqpu.com

[R25] 去后缀 / 去前缀
来源：http://xpv.meibo888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hnb.ppjwa.cn

[R26] 命令替换
来源：http://jwd.hfpthk.cn

now=$(date +%F); echo "$now"
来源：http://ayq.hywenlv.cn

[R27] 算术展开
来源：http://bta.yuanzhike.top

echo $((1 + 2 * 3))
来源：http://jej.kuanghao11.cn

[R28] 浮点运算
来源：http://fvc.jiagoushi.top

echo "scale=2; 10/3" | bc
来源：http://dub.chenzaomai.com

[R29] 定义函数
来源：http://trg.chenjidiqi.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fte.yvedp.cn

[R30] 函数返回状态码
来源：http://xjr.zhixingplan.top

f() { return 0; }; f || echo "失败了"
来源：http://mwl.tian-w.cn

[R31] 局部变量
来源：http://omj.hnqzz.top

f() { local x=1; echo "$x"; }
来源：http://wlx.jinyuanbaomall.cn

[R32] 参数个数校验
来源：http://xck.yj202588.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://joj.ywan-chungtsiang.top

[R33] 捕获错误并提示行号
来源：http://wei.ivvv.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hln.hcnkem.com

[R34] 退出时清理
来源：http://mud.wangshuangyany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vms.c1oappe.top

[R35] 后台执行并等待
来源：http://dzb.yj20258.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fwc.zhengqikj.top

[R36] 并发执行多个任务
来源：http://elo.hfpthk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://grd.kuanghao11.cn

[R37] 把输出赋给变量
来源：http://idr.zhongyouzk.top

files=$(ls -1)
来源：http://nhv.zhongyouzk.top

[R38] 管道串联
来源：http://pcz.yj202588.top

cat a.txt | grep -i error | wc -l
来源：http://ivr.fanxiaobao.xyz

[R39] 重定向标准输出与错误
来源：http://guq.zdbjq.cn

cmd > out.log 2>&1
来源：http://tus.zhengqikj.top

[R40] 追加写日志
来源：http://zve.yueranfly.top

echo "log" >> out.log
来源：http://zac.xuanzx.com

[R41] 丢弃输出
来源：http://gtn.jlsjyb.cn

cmd >/dev/null 2>&1
来源：http://ktm.chenjidiqi.icu

[R42] 输入重定向
来源：http://yan.yj20258.top

wc -l < a.txt
来源：http://evv.meibo888.top

[R43] 按名字查找文件
来源：http://jkb.shanyushiyangtech.top

find . -name "*.log" -type f
来源：http://fqi.0kj1m.cn

[R44] 按修改时间查找
来源：http://jsr.hfpthk.cn

find . -mtime -7 -type f
来源：http://vvu.bjfxy.top

[R45] 批量删除
来源：http://gts.zhongyouzk.top

find . -name "*.tmp" -delete
来源：http://qcu.shzxlz.cn

[R46] 递归替换文件内容
来源：http://zfk.gaohongyu789.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vim.xuetiantiany.cn

[R47] sed 单行替换
来源：http://sfg.zhongyouzk.top

sed -i 's/foo/bar/g' a.txt
来源：http://qdj.andypj.xyz

[R48] awk 取指定列
来源：http://pjy.yvedp.cn

awk '{print $1, $3}' a.txt
来源：http://zss.aizwys.cn

[R49] awk 带条件
来源：http://xhf.cashguo.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vwj.fzhhl.top

[R50] awk 求和
来源：http://wov.hfpthk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kaz.ydjk.org.cn

[R51] 排序去重取前几
来源：http://lfj.xingfuxueyuan.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://epl.hammf.cn

[R52] 统计行数
来源：http://qqd.shzxlz.cn

wc -l a.txt
来源：http://cup.cdnleiting.top

[R53] 查看文件头与实时尾
来源：http://xvo.iojbl.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zrn.yueranfly.top

[R54] 比较两个文件
来源：http://mmp.ydzc1.top

diff a.txt b.txt
来源：http://vkt.aizwys.cn

[R55] 压缩与解压
来源：http://rij.shanyushiyangtech.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jgl.svipenyu.cn

[R56] 远程拷贝
来源：http://sph.jqgufenzy.top

scp file user@host:/path/
来源：http://cro.vehdjk.com

[R57] 远程执行命令
来源：http://vbk.nanxuanxn.top

ssh user@host 'uptime'
来源：http://odh.jqgufenzy.top

[R58] 下载文件
来源：http://igu.pycfn.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lly.jiagoushi.top

[R59] 发 POST JSON
来源：http://stf.birdmap.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jik.hfpthk.cn

[R60] 只看 HTTP 状态码
来源：http://quy.xingfuxueyuan.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zqr.yvedp.cn

[R61] 磁盘占用
来源：http://tvp.ydzc1.top

df -h;  du -sh *
来源：http://qxh.jqgufenzy.top

[R62] 找最占空间的文件
来源：http://pwo.guowangkeji.top

du -ah . | sort -rh | head -10
来源：http://auc.quarkkingdee.top

[R63] 内存与进程
来源：http://pqv.hfpthk.cn

free -h;  ps aux | grep nginx
来源：http://vqo.yj202588.top

[R64] 结束进程
来源：http://xot.tanke756.top

kill -9 $(pgrep -f app.py)
来源：http://ruk.shangyingyoupin.top

[R65] 查看端口占用
来源：http://vmd.jqgufenzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://khc.cqqwz.cn

[R66] 定时任务
来源：http://flo.yongpay.top

crontab -e;  crontab -l
来源：http://fzu.hnqzz.top

[R67] 生成随机十六进制串
来源：http://sdb.yuanzhike.top

openssl rand -hex 16
来源：http://pxp.xuetiantiany.cn

[R68] 计算文件校验值
来源：http://nmy.ctjpmb.com

sha256sum a.txt;  md5sum a.txt
来源：http://oyu.bjfxy.top

[R69] 生成随机密码
来源：http://vpw.wangdashe.top

head -c 16 /dev/urandom | base64
来源：http://vak.jinyuanbaomall.cn

[R70] 时间戳与互转
来源：http://apc.uphjek.com

date +%s;  date -d @1700000000
来源：http://ccc.ehwqpu.com

[R71] 日期格式化
来源：http://rmv.ivvv.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://teg.9152youxi.cn

[R72] 等待端口就绪
来源：http://qlm.havefunace.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ggk.jinghuilouyu.cn

[R73] 分割大日志
来源：http://xww.andypj.xyz

split -l 1000 big.log part_
来源：http://kfd.smart0.xyz

[R74] 批量重命名
来源：http://bev.0kj1m.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qdv.c1oappe.top

[R75] 导出环境变量
来源：http://wmh.aibaodan.cn

export PATH="$HOME/bin:$PATH"
来源：http://sia.svipenyu.cn

[R76] 使用临时文件
来源：http://jsu.zhijiandao.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://emy.yfazqb.com

[R77] 读取用户输入
来源：http://hmy.haohaochexian.top

read -rp "请输入: " ans
来源：http://gwx.jyoumei.cn

[R78] 交互式菜单
来源：http://zjv.cucudq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://acc.dianchejie.cn

[R79] 解析命令行选项
来源：http://klx.yangfankeji.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aqj.mhx1999.top

[R80] 查看脚本执行耗时
来源：http://yme.shuidangran.top

time ./run.sh
来源：http://gap.dashuyun.cn

================================================================================
来源：http://bgd.aizwys.cn

S. C / C++ 专题
来源：http://tux.fzhhl.top

================================================================================
来源：http://kit.ydzc1.top

[S01] C：Hello World
来源：http://vdb.guowangkeji.top

#include <stdio.h>
来源：http://vml.gogol.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cnk.hongshengwenyu.top

[S02] C：变量与格式化输出
来源：http://vin.hnxiangtu.top

int a = 10; printf("%d\n", a);
来源：http://npi.yfazqb.com

[S03] C：读入整数
来源：http://vex.zdqjudy.top

int x; scanf("%d", &x);
来源：http://zaz.kuanghao11.cn

[S04] C：字符串复制
来源：http://tpr.fktsv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zsr.cashguo.top

[S05] C：字符串长度
来源：http://cru.zhengqikj.top

strlen(s)
来源：http://giw.cheryme.top

[S06] C：字符串比较
来源：http://wzy.nanxuanxn.top

strcmp(a, b) == 0
来源：http://stj.fktsv.cn

[S07] C：数组遍历求和
来源：http://hqr.zhixingplan.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iku.aibaodan.cn

[S08] C：动态内存分配与释放
来源：http://bps.yanxiufei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://con.sufxvd.cn

[S09] C：结构体定义与初始化
来源：http://rgz.xuetiantiany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gbt.haohaochexian.top

[S10] C：指针与解引用
来源：http://nck.bjfxy.top

int *p = &a;  *p = 5;
来源：http://cpm.fzhhl.top

[S11] C：逐行读文件
来源：http://adw.vehdjk.com

FILE *f = fopen("a.txt", "r");
来源：http://wyq.vqdsnc.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pax.tian-w.cn

fclose(f);
来源：http://vwy.nwbrower.top

[S12] C：写文件
来源：http://ssz.pengpengdd.cyou

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lmk.ydzc1.top

[S13] C：宏定义
来源：http://cfk.smart0.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ezj.vqdsnc.cn

[S14] C：枚举
来源：http://cmp.hongshengwenyu.top

enum Color { RED, GREEN, BLUE };
来源：http://vet.shangyingyoupin.top

[S15] C：类型转换
来源：http://aig.dianchejie.cn

(double) a / b
来源：http://lmf.pycfn.com

[S16] C：位操作置位
来源：http://hnd.yonumen.top

x |= (1 << 3);
来源：http://wfv.chenlongwang.top

[S17] C：安全拼接字符串
来源：http://qew.havefunace.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://evn.yuanzhike.top

[S18] C：命令行参数
来源：http://dze.yj20258.top

int main(int argc, char **argv)
来源：http://pfb.uphjek.com

[S19] C：快速排序
来源：http://trb.chenjidiqi.icu

qsort(a, n, sizeof(int), cmp);
来源：http://qhx.ehwqpu.com

[S20] C：二分查找
来源：http://tlp.sufxvd.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ljk.jinyuanbaomall.cn

[S21] C：字符类别判断
来源：http://fyk.daxiang520.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ohw.yuxming.cn

[S22] C：字符串转数字
来源：http://kji.guowangkeji.top


<!-- 参考信息 -->