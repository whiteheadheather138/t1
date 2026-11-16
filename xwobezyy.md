代发 wailian999

[Q48] CTE 公用表表达式
来源：http://ifu.hywenlv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cvu.feifeiyinyue.top

SELECT * FROM t WHERE c > 5;
来源：http://hgd.yj20258.top

[Q49] 更新单行
来源：http://pyg.snrcjt.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qrf.ydjk.org.cn

[Q50] 批量更新
来源：http://kmx.fktsv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rkr.yueranfly.top

[Q51] 用子查询更新
来源：http://kxb.cashguo.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kpp.cqqwz.cn

[Q52] 删除指定行
来源：http://fgl.jqgfzy.top

DELETE FROM users WHERE id = 10;
来源：http://icq.0kj1m.cn

[Q53] 按条件删除
来源：http://pqg.pycfn.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jgi.jyoumei.cn

[Q54] 清空表
来源：http://jsk.fengsongda.top

TRUNCATE TABLE logs;
来源：http://hes.sweek.top

[Q55] 排名（并列占位）
来源：http://nyg.chenzaomai.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://usy.feifeiyinyue.top

[Q56] 密集排名（并列不占位）
来源：http://ulx.dianchejie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fmy.cqqwz.cn

[Q57] 行号
来源：http://blx.jqgufenzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cmz.mhx1999.top

[Q58] 累计求和
来源：http://ewf.yangfankeji.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ego.nanxuanxn.top

[Q59] 分组内累计
来源：http://kfp.cdnleiting.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://eye.tian-w.cn

[Q60] 取上一行 / 下一行
来源：http://xxu.hongshengwenyu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://aqb.ppjwa.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://opi.zdbjq.cn

[Q61] 移动平均
来源：http://jbt.hfpthk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://msd.hesvh.cn

[Q62] 分组占比
来源：http://zlz.gzhubu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dji.cucudq.cn

[Q63] 开启事务
来源：http://kza.sjlbkw.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://myx.feifeiyinyue.top

[Q64] 提交事务
来源：http://glo.guowangkeji.top

COMMIT;
来源：http://kvw.birdmap.top

[Q65] 回滚事务
来源：http://coj.hnxiangtu.top

ROLLBACK;
来源：http://cnj.yonumen.top

[Q66] 行锁查询
来源：http://hid.yanxiufei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cro.316326.xyz

[Q67] 设置隔离级别
来源：http://dts.fzhhl.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xtr.iojbl.cn

[Q68] 保存点
来源：http://ayt.wangdashe.top

SAVEPOINT sp1;
来源：http://chh.jlsjyb.cn

ROLLBACK TO sp1;
来源：http://fsy.shuidangran.top

[Q69] 查看执行计划
来源：http://vix.dashuyun.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wcy.jqgufenzy.top

[Q70] 更新统计信息
来源：http://ajc.yuxming.cn

ANALYZE TABLE users;
来源：http://hqh.c1oappe.top

[Q71] 查看建表语句
来源：http://gap.c1oappe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fme.yongpay.top

[Q72] 查看索引
来源：http://mma.kuanghao11.cn

SHOW INDEX FROM users;
来源：http://qdx.pycfn.com

[Q73] 查看表状态
来源：http://tiz.xuanzx.com

SHOW TABLE STATUS LIKE 'users';
来源：http://hmm.jqgfzy.top

[Q74] 强制使用索引
来源：http://fto.zdbjq.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yka.pengpengdd.cyou

[Q75] 日期格式化
来源：http://ruz.yanxiufei.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zgy.yuanzhike.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jnb.c1oappe.top

[Q76] 按天统计
来源：http://znu.aibaodan.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bud.fanxiaobao.xyz

[Q77] 时间加减
来源：http://jtd.meibo888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gon.jyoumei.cn

[Q78] 当前时间
来源：http://kba.tian-w.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aqu.hnqzz.top

[Q79] 字符串拼接
来源：http://nsz.haohaochexian.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ruy.yanxiufei.cn

[Q80] 字符串截取
来源：http://zeb.hammf.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dho.cucudq.cn

[Q81] 字符串替换
来源：http://sam.shzxlz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://osk.daria6918.cn

[Q82] 字符长度与字节长度
来源：http://asx.yanxiufei.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gqq.xuetiantiany.cn

[Q83] 大小写转换
来源：http://wzf.meibo888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yek.svipenyu.cn

[Q84] 去除首尾空格
来源：http://hdd.yanxiufei.cn

SELECT TRIM(name) FROM users;
来源：http://kgg.xylfe.cn

[Q85] 数值取整
来源：http://hyl.sufxvd.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sgd.hfpthk.cn

[Q86] 读取 JSON 字段
来源：http://wfu.xuetiantiany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bye.fehbvm.com

[Q87] JSON 字段做条件
来源：http://jpn.sysykeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rpu.tanke756.top

[Q88] 行转列（条件聚合）
来源：http://pma.tanke756.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ynp.yj20258888.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uto.jinqigufen.top

[Q89] 判断表是否存在
来源：http://mbn.jqgfzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pzr.fktsv.cn

[Q90] 生成序号列
来源：http://hse.vqdsnc.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xup.gaohongyu789.top

================================================================================
来源：http://qvp.sufxvd.cn

R. Bash 专题
来源：http://wia.jianghu66.top

================================================================================
来源：http://lpa.sysykeji.top

[R01] shebang 与严格模式
来源：http://kjr.ivvv.top

#!/usr/bin/env bash
来源：http://hmq.ppjwa.cn

set -euo pipefail
来源：http://nie.hongshengwenyu.top

[R02] 变量赋值与使用
来源：http://lrs.zhiwuduotai.top

name="Tom"; echo "$name"
来源：http://noj.vqdsnc.cn

[R03] 只读变量
来源：http://wnr.zhaomingkeji.xyz

readonly PI=3.14
来源：http://ihy.nwbrower.top

[R04] 位置参数
来源：http://swy.zhijiandao.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ejm.yangfankeji.com

[R05] 参数默认值
来源：http://dal.yongpay.top

name="${1:-default}"
来源：http://zje.pycfn.com

[R06] 判断命令是否存在
来源：http://ewh.xinyue.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yla.aizwys.cn

[R07] if 判断文件
来源：http://yud.kuanghao11.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rhx.zycfv.cn

[R08] 数值比较
来源：http://yim.zdqjudy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cmc.jianghu66.top

[R09] 字符串比较
来源：http://cow.xuanzx.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wpy.yj202588.top

[R10] 正则匹配
来源：http://fsy.jyoumei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lrf.zdbjq.cn

[R11] case 多分支
来源：http://sjt.yuanzhike.top

case "$1" in
来源：http://yav.jyoumei.cn

start) echo "启动" ;;
来源：http://bbx.zycfv.cn

stop)  echo "停止" ;;
来源：http://xaf.vqdsnc.cn

*)     echo "未知命令" ;;
来源：http://moi.epnwcf.com

esac
来源：http://gaf.yuanzhike.top

[R12] for 遍历文件
来源：http://ejb.daxiang520.top

for f in *.txt; do echo "$f"; done
来源：http://kwp.jinqigfzy.top

[R13] for 计数循环
来源：http://xgo.yuanzhike.top

for i in {1..10}; do echo "$i"; done
来源：http://skx.yonumen.top

[R14] C 风格 for
来源：http://iro.jlsjyb.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jwm.ydzc1.top

[R15] while 逐行读文件
来源：http://htu.yueranfly.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://shu.zhixingplan.top

[R16] until 等待条件
来源：http://sod.cqqwz.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fzt.gogol.net.cn

[R17] 数组定义与取值
来源：http://svx.chenlongwang.top

arr=(a b c); echo "${arr[0]}"
来源：http://lvi.fehbvm.com

[R18] 遍历数组
来源：http://ecp.zhongyouzk.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://erf.vehdjk.com

[R19] 数组长度
来源：http://vqt.aibaodan.cn

echo "${#arr[@]}"
来源：http://kgi.xuetiantiany.cn

[R20] 关联数组（字典）
来源：http://akg.ctjpmb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dgm.fehbvm.com

[R21] 字符串长度
来源：http://tcc.jiagoushi.top

echo "${#s}"
来源：http://bjd.chenlongwang.top

[R22] 截取子串
来源：http://uim.zhijiandao.cn

echo "${s:0:5}"
来源：http://iqg.havefunace.top

[R23] 字符串替换
来源：http://mmt.gzhubu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bkk.ivvv.top

[R24] 大小写转换
来源：http://mra.uphjek.com

echo "${s^^}"; echo "${s,,}"
来源：http://nsn.hnqzz.top

[R25] 去后缀 / 去前缀
来源：http://ufo.nwbrower.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://flt.gaohongyu789.top

[R26] 命令替换
来源：http://rao.jinqigufen.top

now=$(date +%F); echo "$now"
来源：http://tro.ydzc1.top

[R27] 算术展开
来源：http://lnm.dashuyun.cn

echo $((1 + 2 * 3))
来源：http://bvl.zhongyouzk.top

[R28] 浮点运算
来源：http://lho.ydjk.org.cn

echo "scale=2; 10/3" | bc
来源：http://ptm.shanyushiyangkeji.top

[R29] 定义函数
来源：http://zht.xuetiantiany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oeb.sweek.top

[R30] 函数返回状态码
来源：http://dgr.316326.xyz

f() { return 0; }; f || echo "失败了"
来源：http://ipr.mhx1999.top

[R31] 局部变量
来源：http://rzp.quarkkingdee.top

f() { local x=1; echo "$x"; }
来源：http://byt.kuanghao11.cn

[R32] 参数个数校验
来源：http://pbe.uphjek.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://thi.ivvv.top

[R33] 捕获错误并提示行号
来源：http://bte.52xcode.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://flr.52xcode.cn

[R34] 退出时清理
来源：http://ewu.chenjidiqi.icu

trap 'rm -f "$tmp"' EXIT
来源：http://rmn.sjlbkw.cn

[R35] 后台执行并等待
来源：http://bqc.quarkkingdee.top

sleep 5 & pid=$!; wait "$pid"
来源：http://awp.hnxiangtu.top

[R36] 并发执行多个任务
来源：http://mcr.jianghu66.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mqb.redwolf501.top

[R37] 把输出赋给变量
来源：http://yue.shangyingyoupin.top

files=$(ls -1)
来源：http://mqy.cucudq.cn

[R38] 管道串联
来源：http://zyz.yvedp.cn

cat a.txt | grep -i error | wc -l
来源：http://qet.feifeiyinyue.top

[R39] 重定向标准输出与错误
来源：http://ksg.xingfuxueyuan.xyz

cmd > out.log 2>&1
来源：http://cgj.jianghu66.top

[R40] 追加写日志
来源：http://eky.fktsv.cn

echo "log" >> out.log
来源：http://nxu.hcnkem.com

[R41] 丢弃输出
来源：http://vmz.yongpay.top

cmd >/dev/null 2>&1
来源：http://cew.chenjidiqi.icu

[R42] 输入重定向
来源：http://pac.ppjwa.cn

wc -l < a.txt
来源：http://fzb.tanke756.top

[R43] 按名字查找文件
来源：http://zva.ctjpmb.com

find . -name "*.log" -type f
来源：http://fqp.yuanzhike.top

[R44] 按修改时间查找
来源：http://cce.havefunace.top

find . -mtime -7 -type f
来源：http://asv.yongpay.top

[R45] 批量删除
来源：http://nlq.ybcxt.top

find . -name "*.tmp" -delete
来源：http://tar.shuidangran.top

[R46] 递归替换文件内容
来源：http://sac.pycfn.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fyh.jqgufenzy.top

[R47] sed 单行替换
来源：http://htn.9152youxi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fkz.gotoacloud.top

[R48] awk 取指定列
来源：http://hts.aizwys.cn

awk '{print $1, $3}' a.txt
来源：http://ayt.zhoulong.xyz

[R49] awk 带条件
来源：http://dbv.ctjpmb.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nbu.bbcook.cn

[R50] awk 求和
来源：http://vzb.mhx1999.top

awk '{s += $2} END {print s}' a.txt
来源：http://phs.ydzc1.top

[R51] 排序去重取前几
来源：http://vml.jianghu66.top

sort a.txt | uniq -c | sort -rn | head
来源：http://xoq.ybcxt.top

[R52] 统计行数
来源：http://ptw.redwolf501.top

wc -l a.txt
来源：http://hjo.jinyuanbaomall.cn

[R53] 查看文件头与实时尾
来源：http://art.ydjk.org.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qaq.hongshengwenyu.top

[R54] 比较两个文件
来源：http://isv.xziqi.cn

diff a.txt b.txt
来源：http://rmg.cucudq.cn

[R55] 压缩与解压
来源：http://rsi.chenjidiqi.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jfn.snrcjt.cn

[R56] 远程拷贝
来源：http://prf.epnwcf.com

scp file user@host:/path/
来源：http://xhh.chenzaomai.com

[R57] 远程执行命令
来源：http://tqm.haohaochexian.top

ssh user@host 'uptime'
来源：http://tvl.birdmap.top

[R58] 下载文件
来源：http://oib.zhaomingkeji.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://edg.jinqigfzy.top

[R59] 发 POST JSON
来源：http://jrx.nwbrower.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://klz.vqdsnc.cn

[R60] 只看 HTTP 状态码
来源：http://wzm.feifeiyinyue.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tgh.tian-w.cn

[R61] 磁盘占用
来源：http://mma.yj20258.top

df -h;  du -sh *
来源：http://cux.gaohongyu789.top

[R62] 找最占空间的文件
来源：http://yit.gotoacloud.top

du -ah . | sort -rh | head -10
来源：http://xhl.shanyushiyangtech.top

[R63] 内存与进程
来源：http://yys.ydjk.org.cn

free -h;  ps aux | grep nginx
来源：http://eew.cheryme.top

[R64] 结束进程
来源：http://frl.ybcxt.top

kill -9 $(pgrep -f app.py)
来源：http://vzg.zhengqikj.top

[R65] 查看端口占用
来源：http://xgh.jinqigufen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qti.hongshengwenyu.top

[R66] 定时任务
来源：http://vse.zhiwuduotai.top

crontab -e;  crontab -l
来源：http://rfu.yuanzhike.top

[R67] 生成随机十六进制串
来源：http://nfj.jyoumei.cn

openssl rand -hex 16
来源：http://cwo.chenlongwang.top

[R68] 计算文件校验值
来源：http://bde.zhiwuduotai.top

sha256sum a.txt;  md5sum a.txt
来源：http://riu.bbcook.cn

[R69] 生成随机密码
来源：http://ade.hysaishi.cn

head -c 16 /dev/urandom | base64
来源：http://nvm.zdbjq.cn

[R70] 时间戳与互转
来源：http://ruw.hnxiangtu.top

date +%s;  date -d @1700000000
来源：http://wez.ehwqpu.com

[R71] 日期格式化
来源：http://txv.sweek.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://eat.fktsv.cn

[R72] 等待端口就绪
来源：http://svq.yanxiufei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vxe.yonumen.top

[R73] 分割大日志
来源：http://bpc.xinyue.icu

split -l 1000 big.log part_
来源：http://yyt.yangfankeji.com

[R74] 批量重命名
来源：http://qxa.cashguo.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dmg.pengpengdd.cyou

[R75] 导出环境变量
来源：http://itj.vqdsnc.cn

export PATH="$HOME/bin:$PATH"
来源：http://zeq.vehdjk.com

[R76] 使用临时文件
来源：http://fpb.chenzaomai.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tcm.ppjwa.cn

[R77] 读取用户输入
来源：http://bci.dianchejie.cn

read -rp "请输入: " ans
来源：http://zfg.ctjpmb.com

[R78] 交互式菜单
来源：http://oyr.birdmap.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hge.vqdsnc.cn

[R79] 解析命令行选项
来源：http://gzx.bjfxy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qpi.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://xhz.kuanghao11.cn

time ./run.sh
来源：http://ohj.xylfe.cn

================================================================================
来源：http://occ.yuxming.cn

S. C / C++ 专题
来源：http://bpx.yangfankeji.com

================================================================================
来源：http://kot.sufxvd.cn

[S01] C：Hello World
来源：http://lko.tian-w.cn

#include <stdio.h>
来源：http://qcz.guowangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ntr.nwbrower.top

[S02] C：变量与格式化输出
来源：http://jdc.sweek.top

int a = 10; printf("%d\n", a);
来源：http://hvd.yueranfly.top

[S03] C：读入整数
来源：http://ggp.0kj1m.cn

int x; scanf("%d", &x);
来源：http://swt.sufxvd.cn

[S04] C：字符串复制
来源：http://ptj.redwolf501.top

char dst[32]; strcpy(dst, "hi");
来源：http://icb.fanxiaobao.xyz

[S05] C：字符串长度
来源：http://hfn.ybcxt.top

strlen(s)
来源：http://rzm.shanyushiyangkeji.top

[S06] C：字符串比较
来源：http://qij.feifeiyinyue.top

strcmp(a, b) == 0
来源：http://bfw.guannengcc.top

[S07] C：数组遍历求和
来源：http://zgl.aizwys.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jma.kuanghao11.cn

[S08] C：动态内存分配与释放
来源：http://gzl.ywan-chungtsiang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://def.cashguo.top

[S09] C：结构体定义与初始化
来源：http://vre.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vpq.fanxiaobao.xyz

[S10] C：指针与解引用
来源：http://kxx.xingfuxueyuan.xyz

int *p = &a;  *p = 5;
来源：http://efn.sjlbkw.cn

[S11] C：逐行读文件
来源：http://ygq.nwbrower.top

FILE *f = fopen("a.txt", "r");
来源：http://gpz.fzhhl.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://uav.jqgufenzy.top

fclose(f);
来源：http://fkp.ybcxt.top

[S12] C：写文件
来源：http://bel.sysykeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://opo.pengpengdd.cyou

[S13] C：宏定义
来源：http://mkt.tanke756.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wfs.aibaodan.cn

[S14] C：枚举
来源：http://lmv.zhiwuduotai.top

enum Color { RED, GREEN, BLUE };
来源：http://psl.wangshuangyany.cn

[S15] C：类型转换
来源：http://ufr.ehwqpu.com

(double) a / b
来源：http://rhs.yfazqb.com

[S16] C：位操作置位
来源：http://hjt.andypj.xyz

x |= (1 << 3);
来源：http://fvy.meibo888.top

[S17] C：安全拼接字符串
来源：http://skr.fengsongda.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vxt.gaohongyu789.top

[S18] C：命令行参数
来源：http://ihr.daxiang520.top


<!-- 参考信息 -->