代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vao.hnqzz.top

[Q52] 删除指定行
来源：http://xcd.ydjk.org.cn

DELETE FROM users WHERE id = 10;
来源：http://omz.snrcjt.cn

[Q53] 按条件删除
来源：http://uwn.chenjidiqi.icu

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ylm.wangdashe.top

[Q54] 清空表
来源：http://ybg.sxryk.cn

TRUNCATE TABLE logs;
来源：http://yqr.nanxuanxn.top

[Q55] 排名（并列占位）
来源：http://xas.smart0.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fup.ywan-chungtsiang.top

[Q56] 密集排名（并列不占位）
来源：http://pfv.tanke756.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gsa.pengpengdd.cyou

[Q57] 行号
来源：http://mrf.hysaishi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gnu.dianchejie.cn

[Q58] 累计求和
来源：http://eay.bbcook.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sgr.havefunace.top

[Q59] 分组内累计
来源：http://gwk.pycfn.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://avy.jinqigfzy.top

[Q60] 取上一行 / 下一行
来源：http://egl.meibo888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zsg.daria6918.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hid.aibaodan.cn

[Q61] 移动平均
来源：http://hfr.daria6918.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tyh.birdmap.top

[Q62] 分组占比
来源：http://lhq.xuanzx.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nfh.sufxvd.cn

[Q63] 开启事务
来源：http://gad.xuetiantiany.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://uqa.zhixingplan.top

[Q64] 提交事务
来源：http://ayg.shangyingyoupin.top

COMMIT;
来源：http://nzg.havefunace.top

[Q65] 回滚事务
来源：http://epi.hysaishi.cn

ROLLBACK;
来源：http://ffc.cheryme.top

[Q66] 行锁查询
来源：http://dud.cqqwz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sjc.redwolf501.top

[Q67] 设置隔离级别
来源：http://rio.svipenyu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qam.sjlbkw.cn

[Q68] 保存点
来源：http://nts.birdmap.top

SAVEPOINT sp1;
来源：http://brs.xziqi.cn

ROLLBACK TO sp1;
来源：http://zcn.hesvh.cn

[Q69] 查看执行计划
来源：http://nqa.yvedp.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mkz.tarul.cn

[Q70] 更新统计信息
来源：http://spz.svipenyu.cn

ANALYZE TABLE users;
来源：http://yor.feifeiyinyue.top

[Q71] 查看建表语句
来源：http://plv.yonumen.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xgc.ppjwa.cn

[Q72] 查看索引
来源：http://mlm.jinqigufen.top

SHOW INDEX FROM users;
来源：http://wuw.tanke756.top

[Q73] 查看表状态
来源：http://vqk.fehbvm.com

SHOW TABLE STATUS LIKE 'users';
来源：http://tvu.nanxuanxn.top

[Q74] 强制使用索引
来源：http://cqj.wangdashe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nmt.fehbvm.com

[Q75] 日期格式化
来源：http://hkg.zhongyouzk.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jcj.ydjk.org.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dia.chenjidiqi.icu

[Q76] 按天统计
来源：http://bst.shanyushiyangtech.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://goq.sxryk.cn

[Q77] 时间加减
来源：http://pem.epnwcf.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://acl.zhixingplan.top

[Q78] 当前时间
来源：http://two.tianlin.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yqc.bjfxy.top

[Q79] 字符串拼接
来源：http://erl.cucudq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qtp.hammf.cn

[Q80] 字符串截取
来源：http://jfm.xuanzx.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jtk.sufxvd.cn

[Q81] 字符串替换
来源：http://wny.fzhhl.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nvo.aizwys.cn

[Q82] 字符长度与字节长度
来源：http://rix.gzhubu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lxq.ydzc1.top

[Q83] 大小写转换
来源：http://owl.wangshuangyany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tkf.yongpay.top

[Q84] 去除首尾空格
来源：http://bny.hongshengwenyu.top

SELECT TRIM(name) FROM users;
来源：http://euo.shuidangran.top

[Q85] 数值取整
来源：http://aiv.havefunace.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ojq.jinghuilouyu.cn

[Q86] 读取 JSON 字段
来源：http://fyz.xinyue.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nlt.jinyuanbaomall.cn

[Q87] JSON 字段做条件
来源：http://bbe.yanxiufei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mxv.gzhubu.top

[Q88] 行转列（条件聚合）
来源：http://jyd.bbcook.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rwf.sxryk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xbx.zhijiandao.cn

[Q89] 判断表是否存在
来源：http://riu.mhx1999.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lgy.vqdsnc.cn

[Q90] 生成序号列
来源：http://uok.jqgufenzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vcs.dashuyun.cn

================================================================================
来源：http://eyw.cucudq.cn

R. Bash 专题
来源：http://dfq.zhengqikj.top

================================================================================
来源：http://iuk.zhoulong.xyz

[R01] shebang 与严格模式
来源：http://ncg.vehdjk.com

#!/usr/bin/env bash
来源：http://oew.yangfankeji.com

set -euo pipefail
来源：http://rka.cashguo.top

[R02] 变量赋值与使用
来源：http://hbw.redwolf501.top

name="Tom"; echo "$name"
来源：http://nyd.smart0.xyz

[R03] 只读变量
来源：http://syq.pengpengdd.cyou

readonly PI=3.14
来源：http://dvb.sysykeji.top

[R04] 位置参数
来源：http://ulu.sxryk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fnq.0kj1m.cn

[R05] 参数默认值
来源：http://jvu.hammf.cn

name="${1:-default}"
来源：http://cqi.shzxlz.cn

[R06] 判断命令是否存在
来源：http://ked.yangfankeji.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fco.ywan-chungtsiang.top

[R07] if 判断文件
来源：http://dmt.52xcode.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bma.xuetiantiany.cn

[R08] 数值比较
来源：http://jgt.aizwys.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zlh.yuanzhike.top

[R09] 字符串比较
来源：http://yau.vehdjk.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yow.shuidangran.top

[R10] 正则匹配
来源：http://mio.hfpthk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tjo.snrcjt.cn

[R11] case 多分支
来源：http://huk.zhengqikj.top

case "$1" in
来源：http://uzk.jinghuilouyu.cn

start) echo "启动" ;;
来源：http://pft.jianghu66.top

stop)  echo "停止" ;;
来源：http://yyt.jqgufenzy.top

*)     echo "未知命令" ;;
来源：http://lta.zhongyouzk.top

esac
来源：http://jai.9152youxi.cn

[R12] for 遍历文件
来源：http://nez.fzhhl.top

for f in *.txt; do echo "$f"; done
来源：http://nsy.iojbl.cn

[R13] for 计数循环
来源：http://ocm.jinqigufen.top

for i in {1..10}; do echo "$i"; done
来源：http://wau.birdmap.top

[R14] C 风格 for
来源：http://gpj.ydzc1.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oku.epnwcf.com

[R15] while 逐行读文件
来源：http://pfv.tianlin.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://orq.yfazqb.com

[R16] until 等待条件
来源：http://gbi.andypj.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xgq.chenzaomai.com

[R17] 数组定义与取值
来源：http://ioi.yj202588.top

arr=(a b c); echo "${arr[0]}"
来源：http://dye.vqdsnc.cn

[R18] 遍历数组
来源：http://usb.daria6918.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nja.zhengqikj.top

[R19] 数组长度
来源：http://nbr.ivvv.top

echo "${#arr[@]}"
来源：http://qoj.guowangkeji.top

[R20] 关联数组（字典）
来源：http://wrg.haohaochexian.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://axp.gotoacloud.top

[R21] 字符串长度
来源：http://fqq.nanxuanxn.top

echo "${#s}"
来源：http://vuf.xylfe.cn

[R22] 截取子串
来源：http://zqk.havefunace.top

echo "${s:0:5}"
来源：http://rfw.aizwys.cn

[R23] 字符串替换
来源：http://lch.ivvv.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ykr.fehbvm.com

[R24] 大小写转换
来源：http://mwp.sysykeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://hmn.jinyuanbaomall.cn

[R25] 去后缀 / 去前缀
来源：http://bbv.gzhubu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://faa.316326.xyz

[R26] 命令替换
来源：http://uzg.hywenlv.cn

now=$(date +%F); echo "$now"
来源：http://dqc.epnwcf.com

[R27] 算术展开
来源：http://ydi.daria6918.cn

echo $((1 + 2 * 3))
来源：http://eqh.shangyingyoupin.top

[R28] 浮点运算
来源：http://ntr.ehwqpu.com

echo "scale=2; 10/3" | bc
来源：http://obj.0kj1m.cn

[R29] 定义函数
来源：http://jtg.yfazqb.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hof.316326.xyz

[R30] 函数返回状态码
来源：http://svf.yj202588.top

f() { return 0; }; f || echo "失败了"
来源：http://xub.epnwcf.com

[R31] 局部变量
来源：http://ahg.yanxiufei.cn

f() { local x=1; echo "$x"; }
来源：http://fhj.tarul.cn

[R32] 参数个数校验
来源：http://kwc.gaohongyu789.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://neb.jqgfzy.top

[R33] 捕获错误并提示行号
来源：http://afg.yonumen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qea.zhixingplan.top

[R34] 退出时清理
来源：http://szs.mhx1999.top

trap 'rm -f "$tmp"' EXIT
来源：http://kqn.jinyuanbaomall.cn

[R35] 后台执行并等待
来源：http://nnq.nwbrower.top

sleep 5 & pid=$!; wait "$pid"
来源：http://lel.mhx1999.top

[R36] 并发执行多个任务
来源：http://ijj.ybcxt.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bor.c1oappe.top

[R37] 把输出赋给变量
来源：http://thd.ivvv.top

files=$(ls -1)
来源：http://uhs.vehdjk.com

[R38] 管道串联
来源：http://woj.zhongyouzk.top

cat a.txt | grep -i error | wc -l
来源：http://ply.cashguo.top

[R39] 重定向标准输出与错误
来源：http://vhi.hesvh.cn

cmd > out.log 2>&1
来源：http://lzh.yfazqb.com

[R40] 追加写日志
来源：http://vgn.feifeiyinyue.top

echo "log" >> out.log
来源：http://crj.jinyuanbaomall.cn

[R41] 丢弃输出
来源：http://oev.uphjek.com

cmd >/dev/null 2>&1
来源：http://cjn.daria6918.cn

[R42] 输入重定向
来源：http://hbi.chenjidiqi.icu

wc -l < a.txt
来源：http://kgd.nwbrower.top

[R43] 按名字查找文件
来源：http://kbb.andypj.xyz

find . -name "*.log" -type f
来源：http://rko.sweek.top

[R44] 按修改时间查找
来源：http://nze.bjfxy.top

find . -mtime -7 -type f
来源：http://ovt.smart0.xyz

[R45] 批量删除
来源：http://bzm.xylfe.cn

find . -name "*.tmp" -delete
来源：http://tml.xziqi.cn

[R46] 递归替换文件内容
来源：http://hgj.jqgufenzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tbb.havefunace.top

[R47] sed 单行替换
来源：http://vjw.jianghu66.top

sed -i 's/foo/bar/g' a.txt
来源：http://vta.jlsjyb.cn

[R48] awk 取指定列
来源：http://tkl.0kj1m.cn

awk '{print $1, $3}' a.txt
来源：http://fbs.pycfn.com

[R49] awk 带条件
来源：http://ktu.cucudq.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gqi.wangdashe.top

[R50] awk 求和
来源：http://vjb.xinyue.icu

awk '{s += $2} END {print s}' a.txt
来源：http://lix.jqgfzy.top

[R51] 排序去重取前几
来源：http://pnn.fanxiaobao.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://swp.fzhhl.top

[R52] 统计行数
来源：http://nku.fanxiaobao.xyz

wc -l a.txt
来源：http://pnz.chenjidiqi.icu

[R53] 查看文件头与实时尾
来源：http://sln.fzhhl.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kas.gogol.net.cn

[R54] 比较两个文件
来源：http://jcx.jinqigufen.top

diff a.txt b.txt
来源：http://lov.ppjwa.cn

[R55] 压缩与解压
来源：http://xhv.smart0.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kmr.nanxuanxn.top

[R56] 远程拷贝
来源：http://orh.9152youxi.cn

scp file user@host:/path/
来源：http://fjh.yj202588.top

[R57] 远程执行命令
来源：http://rmm.cucudq.cn

ssh user@host 'uptime'
来源：http://koi.shanyushiyangkeji.top

[R58] 下载文件
来源：http://ota.gotoacloud.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wkr.tianlin.xyz

[R59] 发 POST JSON
来源：http://oqy.hywenlv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ufe.feifeiyinyue.top

[R60] 只看 HTTP 状态码
来源：http://qfr.52xcode.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://unp.shzxlz.cn

[R61] 磁盘占用
来源：http://gju.iojbl.cn

df -h;  du -sh *
来源：http://aof.havefunace.top

[R62] 找最占空间的文件
来源：http://hdf.ehwqpu.com

du -ah . | sort -rh | head -10
来源：http://bju.ctjpmb.com

[R63] 内存与进程
来源：http://osp.xinyue.icu

free -h;  ps aux | grep nginx
来源：http://uvq.yanxiufei.cn

[R64] 结束进程
来源：http://nka.sxryk.cn

kill -9 $(pgrep -f app.py)
来源：http://mgo.dashuyun.cn

[R65] 查看端口占用
来源：http://ayp.gaohongyu789.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gyj.yongpay.top

[R66] 定时任务
来源：http://gfv.shanyushiyangkeji.top

crontab -e;  crontab -l
来源：http://wpm.fengsongda.top

[R67] 生成随机十六进制串
来源：http://spq.andypj.xyz

openssl rand -hex 16
来源：http://phj.iojbl.cn

[R68] 计算文件校验值
来源：http://qmx.ctjpmb.com

sha256sum a.txt;  md5sum a.txt
来源：http://zfe.hysaishi.cn

[R69] 生成随机密码
来源：http://tza.sysykeji.top

head -c 16 /dev/urandom | base64
来源：http://hfz.havefunace.top

[R70] 时间戳与互转
来源：http://fzd.xylfe.cn

date +%s;  date -d @1700000000
来源：http://fpq.yj20258.top

[R71] 日期格式化
来源：http://efn.yvedp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nqu.dashuyun.cn

[R72] 等待端口就绪
来源：http://rnh.fengsongda.top

until nc -z localhost 3306; do sleep 1; done
来源：http://spg.52xcode.cn

[R73] 分割大日志
来源：http://pdj.zhixingplan.top

split -l 1000 big.log part_
来源：http://dai.ydzc1.top

[R74] 批量重命名
来源：http://ohn.aibaodan.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kmq.yangfankeji.com

[R75] 导出环境变量
来源：http://gdd.yj20258.top

export PATH="$HOME/bin:$PATH"
来源：http://hwq.dianchejie.cn

[R76] 使用临时文件
来源：http://dna.haohaochexian.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://edn.dashuyun.cn

[R77] 读取用户输入
来源：http://swb.sweek.top

read -rp "请输入: " ans
来源：http://gnd.shanyushiyangtech.top

[R78] 交互式菜单
来源：http://ubq.hfpthk.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fqt.fktsv.cn

[R79] 解析命令行选项
来源：http://etw.aizwys.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ntp.jinqigufen.top

[R80] 查看脚本执行耗时
来源：http://wey.hnxiangtu.top

time ./run.sh
来源：http://rzr.hnqzz.top

================================================================================
来源：http://ubx.yangfankeji.com

S. C / C++ 专题
来源：http://ecf.shuidangran.top

================================================================================
来源：http://hpn.yonumen.top

[S01] C：Hello World
来源：http://uqs.bjfxy.top

#include <stdio.h>
来源：http://wcs.gotoacloud.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jpr.yangfankeji.com

[S02] C：变量与格式化输出
来源：http://bmt.jqgfzy.top

int a = 10; printf("%d\n", a);
来源：http://rth.epnwcf.com

[S03] C：读入整数
来源：http://saw.52xcode.cn

int x; scanf("%d", &x);
来源：http://big.shzxlz.cn

[S04] C：字符串复制
来源：http://msr.fzhhl.top

char dst[32]; strcpy(dst, "hi");
来源：http://rlq.nanxuanxn.top

[S05] C：字符串长度
来源：http://yws.zdqjudy.top

strlen(s)
来源：http://hco.xylfe.cn

[S06] C：字符串比较
来源：http://ggg.chenjidiqi.icu

strcmp(a, b) == 0
来源：http://rcg.yueranfly.top

[S07] C：数组遍历求和
来源：http://rsv.dashuyun.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://its.epnwcf.com

[S08] C：动态内存分配与释放
来源：http://iic.zhongyouzk.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mvv.sxryk.cn

[S09] C：结构体定义与初始化
来源：http://eho.tian-w.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zoi.yfazqb.com

[S10] C：指针与解引用
来源：http://vau.daxiang520.top

int *p = &a;  *p = 5;
来源：http://grp.gzhubu.top

[S11] C：逐行读文件
来源：http://lrk.cheryme.top

FILE *f = fopen("a.txt", "r");
来源：http://fwc.0kj1m.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://szd.wangshuangyany.cn

fclose(f);
来源：http://thx.birdmap.top

[S12] C：写文件
来源：http://rdl.dianchejie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://syd.wangdashe.top

[S13] C：宏定义
来源：http://mrh.hywenlv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jkg.yueranfly.top

[S14] C：枚举
来源：http://nvn.yfazqb.com

enum Color { RED, GREEN, BLUE };
来源：http://mdl.yanxiufei.cn

[S15] C：类型转换
来源：http://pjv.zhoulong.xyz

(double) a / b
来源：http://ojb.tian-w.cn

[S16] C：位操作置位
来源：http://zjy.xuetiantiany.cn

x |= (1 << 3);
来源：http://tqc.zhongyouzk.top

[S17] C：安全拼接字符串
来源：http://bjl.yangfankeji.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://txg.iojbl.cn

[S18] C：命令行参数
来源：http://kbu.daxiang520.top

int main(int argc, char **argv)
来源：http://vvm.shanyushiyangtech.top

[S19] C：快速排序
来源：http://rkq.xuanzx.com

qsort(a, n, sizeof(int), cmp);
来源：http://lff.vehdjk.com

[S20] C：二分查找
来源：http://dcf.jiagoushi.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://voc.hongshengwenyu.top

[S21] C：字符类别判断
来源：http://dwq.birdmap.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://olb.vqdsnc.cn

[S22] C：字符串转数字
来源：http://exc.shuidangran.top


<!-- 参考信息 -->