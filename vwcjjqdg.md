代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nlf.hesvh.cn

[Q50] 批量更新
来源：http://xcw.zhiwuduotai.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://acx.cheryme.top

[Q51] 用子查询更新
来源：http://rjz.jiagoushi.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://opb.smart0.xyz

[Q52] 删除指定行
来源：http://gmg.yanxiufei.cn

DELETE FROM users WHERE id = 10;
来源：http://ncc.tian-w.cn

[Q53] 按条件删除
来源：http://ddr.shangyingyoupin.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wbg.shanyushiyangkeji.top

[Q54] 清空表
来源：http://arj.vqdsnc.cn

TRUNCATE TABLE logs;
来源：http://tdj.shzxlz.cn

[Q55] 排名（并列占位）
来源：http://heb.9152youxi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qqv.yuxming.cn

[Q56] 密集排名（并列不占位）
来源：http://dew.ehwqpu.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://osb.shzxlz.cn

[Q57] 行号
来源：http://pfl.c1oappe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://riz.yueranfly.top

[Q58] 累计求和
来源：http://dhh.zhongyouzk.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nyw.bjfxy.top

[Q59] 分组内累计
来源：http://cgy.shanyushiyangtech.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ylx.fzhhl.top

[Q60] 取上一行 / 下一行
来源：http://ozh.zdqjudy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xuu.aibaodan.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hlt.sweek.top

[Q61] 移动平均
来源：http://sgx.yuxming.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qyw.pycfn.com

[Q62] 分组占比
来源：http://msn.jinqigfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vyx.jinghuilouyu.cn

[Q63] 开启事务
来源：http://ebe.nwbrower.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fao.cdnleiting.top

[Q64] 提交事务
来源：http://pai.yfazqb.com

COMMIT;
来源：http://srp.cheryme.top

[Q65] 回滚事务
来源：http://qvp.52xcode.cn

ROLLBACK;
来源：http://ave.xziqi.cn

[Q66] 行锁查询
来源：http://pjg.fengsongda.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fgt.daria6918.cn

[Q67] 设置隔离级别
来源：http://qxe.sufxvd.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://phb.haohaochexian.top

[Q68] 保存点
来源：http://deb.hammf.cn

SAVEPOINT sp1;
来源：http://vwv.hnqzz.top

ROLLBACK TO sp1;
来源：http://nra.yfazqb.com

[Q69] 查看执行计划
来源：http://bir.nwbrower.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tdm.jlsjyb.cn

[Q70] 更新统计信息
来源：http://jrg.meibo888.top

ANALYZE TABLE users;
来源：http://lme.shanyushiyangtech.top

[Q71] 查看建表语句
来源：http://zzx.yj20258.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eft.52xcode.cn

[Q72] 查看索引
来源：http://pzl.zycfv.cn

SHOW INDEX FROM users;
来源：http://wgo.snrcjt.cn

[Q73] 查看表状态
来源：http://ift.ybcxt.top

SHOW TABLE STATUS LIKE 'users';
来源：http://thp.c1oappe.top

[Q74] 强制使用索引
来源：http://axq.hnqzz.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://act.hongshengwenyu.top

[Q75] 日期格式化
来源：http://kpv.zdbjq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rre.gzhubu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sqi.yangfankeji.com

[Q76] 按天统计
来源：http://wpx.snrcjt.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ndu.tian-w.cn

[Q77] 时间加减
来源：http://bst.yj20258.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vyt.zhongyouzk.top

[Q78] 当前时间
来源：http://mai.tanke756.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vtj.aibaodan.cn

[Q79] 字符串拼接
来源：http://vmn.jlsjyb.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ory.tanke756.top

[Q80] 字符串截取
来源：http://cqp.hywenlv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vwq.sufxvd.cn

[Q81] 字符串替换
来源：http://srd.feifeiyinyue.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tiu.yfazqb.com

[Q82] 字符长度与字节长度
来源：http://cgo.hongshengwenyu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gsb.yfazqb.com

[Q83] 大小写转换
来源：http://mdg.svipenyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://meb.aibaodan.cn

[Q84] 去除首尾空格
来源：http://hni.ywan-chungtsiang.top

SELECT TRIM(name) FROM users;
来源：http://bth.pengpengdd.cyou

[Q85] 数值取整
来源：http://uoz.zycfv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hpe.tian-w.cn

[Q86] 读取 JSON 字段
来源：http://hop.jqgufenzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bvz.hcnkem.com

[Q87] JSON 字段做条件
来源：http://gtp.zdbjq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sxi.svipenyu.cn

[Q88] 行转列（条件聚合）
来源：http://uys.feifeiyinyue.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nwa.hysaishi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lxp.meibo888.top

[Q89] 判断表是否存在
来源：http://fns.shanyushiyangtech.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dmw.shzxlz.cn

[Q90] 生成序号列
来源：http://xdr.zdqjudy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qsi.xingfuxueyuan.xyz

================================================================================
来源：http://qzg.zhaomingkeji.xyz

R. Bash 专题
来源：http://pvl.vehdjk.com

================================================================================
来源：http://roh.ctjpmb.com

[R01] shebang 与严格模式
来源：http://kxc.uphjek.com

#!/usr/bin/env bash
来源：http://rsi.jyoumei.cn

set -euo pipefail
来源：http://uve.zdqjudy.top

[R02] 变量赋值与使用
来源：http://nbi.aizwys.cn

name="Tom"; echo "$name"
来源：http://jyw.yj202588.top

[R03] 只读变量
来源：http://lxw.daria6918.cn

readonly PI=3.14
来源：http://fjp.hcnkem.com

[R04] 位置参数
来源：http://gjs.cashguo.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xra.yfazqb.com

[R05] 参数默认值
来源：http://aln.zdqjudy.top

name="${1:-default}"
来源：http://sci.vehdjk.com

[R06] 判断命令是否存在
来源：http://rak.0kj1m.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hhq.ctjpmb.com

[R07] if 判断文件
来源：http://dth.cashguo.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yct.yj20258888.top

[R08] 数值比较
来源：http://rci.cucudq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zgp.andypj.xyz

[R09] 字符串比较
来源：http://aco.birdmap.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cbz.xinyue.icu

[R10] 正则匹配
来源：http://hlz.guowangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pfd.feifeiyinyue.top

[R11] case 多分支
来源：http://ukz.ydjk.org.cn

case "$1" in
来源：http://hlq.birdmap.top

start) echo "启动" ;;
来源：http://lvx.ydzc1.top

stop)  echo "停止" ;;
来源：http://eme.cashguo.top

*)     echo "未知命令" ;;
来源：http://doe.vehdjk.com

esac
来源：http://tcf.tarul.cn

[R12] for 遍历文件
来源：http://alm.aibaodan.cn

for f in *.txt; do echo "$f"; done
来源：http://wga.sufxvd.cn

[R13] for 计数循环
来源：http://uka.vehdjk.com

for i in {1..10}; do echo "$i"; done
来源：http://kne.sysykeji.top

[R14] C 风格 for
来源：http://miq.sxryk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hil.iojbl.cn

[R15] while 逐行读文件
来源：http://mrw.hysaishi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://buj.gaohongyu789.top

[R16] until 等待条件
来源：http://dij.316326.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mbt.meibo888.top

[R17] 数组定义与取值
来源：http://vbo.316326.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://unu.wangshuangyany.cn

[R18] 遍历数组
来源：http://pke.ctjpmb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rhz.cqqwz.cn

[R19] 数组长度
来源：http://oez.wangdashe.top

echo "${#arr[@]}"
来源：http://haa.tian-w.cn

[R20] 关联数组（字典）
来源：http://wnb.bjfxy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wxs.cucudq.cn

[R21] 字符串长度
来源：http://sac.daria6918.cn

echo "${#s}"
来源：http://ymy.gzhubu.top

[R22] 截取子串
来源：http://sdi.pengpengdd.cyou

echo "${s:0:5}"
来源：http://rme.gaohongyu789.top

[R23] 字符串替换
来源：http://gns.yuanzhike.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ilk.dianchejie.cn

[R24] 大小写转换
来源：http://fjx.yonumen.top

echo "${s^^}"; echo "${s,,}"
来源：http://iot.ppjwa.cn

[R25] 去后缀 / 去前缀
来源：http://xpu.kuanghao11.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pgj.shanyushiyangkeji.top

[R26] 命令替换
来源：http://ger.redwolf501.top

now=$(date +%F); echo "$now"
来源：http://jpz.yfazqb.com

[R27] 算术展开
来源：http://iqu.shangyingyoupin.top

echo $((1 + 2 * 3))
来源：http://vez.shangyingyoupin.top

[R28] 浮点运算
来源：http://uur.nanxinkj.top

echo "scale=2; 10/3" | bc
来源：http://qwz.guannengcc.top

[R29] 定义函数
来源：http://sbb.zhixingplan.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://thy.yanxiufei.cn

[R30] 函数返回状态码
来源：http://kgq.yj202588.top

f() { return 0; }; f || echo "失败了"
来源：http://pad.zdbjq.cn

[R31] 局部变量
来源：http://ylk.snrcjt.cn

f() { local x=1; echo "$x"; }
来源：http://poc.zhengqikj.top

[R32] 参数个数校验
来源：http://ffc.zhoulong.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ehi.dianchejie.cn

[R33] 捕获错误并提示行号
来源：http://epw.smart0.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ubi.jinghuilouyu.cn

[R34] 退出时清理
来源：http://ifi.chenjidiqi.icu

trap 'rm -f "$tmp"' EXIT
来源：http://ktd.shzxlz.cn

[R35] 后台执行并等待
来源：http://thw.sxryk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kua.yuanzhike.top

[R36] 并发执行多个任务
来源：http://vtf.ctjpmb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qnv.jinyuanbaomall.cn

[R37] 把输出赋给变量
来源：http://hdz.aibaodan.cn

files=$(ls -1)
来源：http://yva.zhengqikj.top

[R38] 管道串联
来源：http://lbi.gogol.net.cn

cat a.txt | grep -i error | wc -l
来源：http://skg.fengsongda.top

[R39] 重定向标准输出与错误
来源：http://jxl.guannengcc.top

cmd > out.log 2>&1
来源：http://wyo.jinqigufen.top

[R40] 追加写日志
来源：http://qgd.wangshuangyany.cn

echo "log" >> out.log
来源：http://wgy.nwbrower.top

[R41] 丢弃输出
来源：http://qfb.quarkkingdee.top

cmd >/dev/null 2>&1
来源：http://ejf.hnqzz.top

[R42] 输入重定向
来源：http://gmu.vqdsnc.cn

wc -l < a.txt
来源：http://hwk.smart0.xyz

[R43] 按名字查找文件
来源：http://ypx.zdbjq.cn

find . -name "*.log" -type f
来源：http://pak.bbcook.cn

[R44] 按修改时间查找
来源：http://vbm.haohaochexian.top

find . -mtime -7 -type f
来源：http://avq.haohaochexian.top

[R45] 批量删除
来源：http://ihg.c1oappe.top

find . -name "*.tmp" -delete
来源：http://ekg.ydjk.org.cn

[R46] 递归替换文件内容
来源：http://oey.sweek.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xdz.zhixingplan.top

[R47] sed 单行替换
来源：http://zwb.sufxvd.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hsv.dashuyun.cn

[R48] awk 取指定列
来源：http://pqb.jinyuanbaomall.cn

awk '{print $1, $3}' a.txt
来源：http://yky.fzhhl.top

[R49] awk 带条件
来源：http://yth.hongshengwenyu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zvs.tian-w.cn

[R50] awk 求和
来源：http://qas.iojbl.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mny.xingfuxueyuan.xyz

[R51] 排序去重取前几
来源：http://wdz.fengsongda.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ran.tarul.cn

[R52] 统计行数
来源：http://zwe.fehbvm.com

wc -l a.txt
来源：http://vzw.jyoumei.cn

[R53] 查看文件头与实时尾
来源：http://ogz.shanyushiyangtech.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://eaw.xingfuxueyuan.xyz

[R54] 比较两个文件
来源：http://ovz.xinyue.icu

diff a.txt b.txt
来源：http://mxw.jinyuanbaomall.cn

[R55] 压缩与解压
来源：http://whs.kuanghao11.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://akq.fktsv.cn

[R56] 远程拷贝
来源：http://llq.snrcjt.cn

scp file user@host:/path/
来源：http://kcs.sufxvd.cn

[R57] 远程执行命令
来源：http://qva.hfpthk.cn

ssh user@host 'uptime'
来源：http://zoa.nwbrower.top

[R58] 下载文件
来源：http://hxz.shanyushiyangkeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kbk.hfpthk.cn

[R59] 发 POST JSON
来源：http://lfm.hongshengwenyu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://arn.guannengcc.top

[R60] 只看 HTTP 状态码
来源：http://xhl.meibo888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://epm.yj202588.top

[R61] 磁盘占用
来源：http://xyx.cqqwz.cn

df -h;  du -sh *
来源：http://sgx.quarkkingdee.top

[R62] 找最占空间的文件
来源：http://aoc.epnwcf.com

du -ah . | sort -rh | head -10
来源：http://ftz.dianchejie.cn

[R63] 内存与进程
来源：http://eky.guannengcc.top

free -h;  ps aux | grep nginx
来源：http://rwh.daria6918.cn

[R64] 结束进程
来源：http://wwt.yj20258.top

kill -9 $(pgrep -f app.py)
来源：http://mey.gaohongyu789.top

[R65] 查看端口占用
来源：http://tfa.wangshuangyany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hgr.zdqjudy.top

[R66] 定时任务
来源：http://phb.zhiwuduotai.top

crontab -e;  crontab -l
来源：http://hso.zhixingplan.top

[R67] 生成随机十六进制串
来源：http://jul.haohaochexian.top

openssl rand -hex 16
来源：http://kum.jinqigufen.top

[R68] 计算文件校验值
来源：http://lhy.nwbrower.top

sha256sum a.txt;  md5sum a.txt
来源：http://ino.zhengqikj.top

[R69] 生成随机密码
来源：http://cil.nwbrower.top

head -c 16 /dev/urandom | base64
来源：http://mge.vehdjk.com

[R70] 时间戳与互转
来源：http://mgs.hnxiangtu.top

date +%s;  date -d @1700000000
来源：http://nvs.nanxinkj.top

[R71] 日期格式化
来源：http://nzj.cucudq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hkm.cdnleiting.top

[R72] 等待端口就绪
来源：http://bbc.tanke756.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fvd.quarkkingdee.top

[R73] 分割大日志
来源：http://mxr.c1oappe.top

split -l 1000 big.log part_
来源：http://bau.ctjpmb.com

[R74] 批量重命名
来源：http://obx.gaohongyu789.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tbs.cucudq.cn

[R75] 导出环境变量
来源：http://sma.zycfv.cn

export PATH="$HOME/bin:$PATH"
来源：http://gwb.shanyushiyangkeji.top

[R76] 使用临时文件
来源：http://fli.hnxiangtu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://alk.xziqi.cn

[R77] 读取用户输入
来源：http://lld.fktsv.cn

read -rp "请输入: " ans
来源：http://fku.shanyushiyangtech.top

[R78] 交互式菜单
来源：http://nke.pengpengdd.cyou

select opt in a b c; do echo "$opt"; break; done
来源：http://ccl.yangfankeji.com

[R79] 解析命令行选项
来源：http://ywn.zhongyouzk.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ine.hywenlv.cn

[R80] 查看脚本执行耗时
来源：http://uyj.ivvv.top

time ./run.sh
来源：http://ktr.jqgfzy.top

================================================================================
来源：http://qmf.fanxiaobao.xyz

S. C / C++ 专题
来源：http://cev.chenzaomai.com

================================================================================
来源：http://uqj.ybcxt.top

[S01] C：Hello World
来源：http://rpi.zhaomingkeji.xyz

#include <stdio.h>
来源：http://qlm.jinqigufen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wky.yj20258888.top

[S02] C：变量与格式化输出
来源：http://vzz.meibo888.top

int a = 10; printf("%d\n", a);
来源：http://ysg.wangdashe.top

[S03] C：读入整数
来源：http://xpe.hywenlv.cn

int x; scanf("%d", &x);
来源：http://wmm.shzxlz.cn

[S04] C：字符串复制
来源：http://gqp.xylfe.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ayx.iojbl.cn

[S05] C：字符串长度
来源：http://irf.jinqigfzy.top

strlen(s)
来源：http://gaq.chenzaomai.com

[S06] C：字符串比较
来源：http://yqo.yfazqb.com

strcmp(a, b) == 0
来源：http://ere.quarkkingdee.top

[S07] C：数组遍历求和
来源：http://bxa.redwolf501.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yys.hywenlv.cn

[S08] C：动态内存分配与释放
来源：http://qjp.sysykeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mch.yuanzhike.top

[S09] C：结构体定义与初始化
来源：http://tda.cucudq.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xya.sysykeji.top

[S10] C：指针与解引用
来源：http://brq.aizwys.cn

int *p = &a;  *p = 5;
来源：http://ytz.wangshuangyany.cn

[S11] C：逐行读文件
来源：http://glc.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "r");
来源：http://aue.wangdashe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xas.fanxiaobao.xyz

fclose(f);
来源：http://omv.zhongyouzk.top

[S12] C：写文件
来源：http://fwu.yanxiufei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qvb.snrcjt.cn

[S13] C：宏定义
来源：http://ufe.aibaodan.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bgf.jyoumei.cn

[S14] C：枚举
来源：http://ojx.yueranfly.top

enum Color { RED, GREEN, BLUE };
来源：http://rus.hongshengwenyu.top

[S15] C：类型转换
来源：http://fzt.bjfxy.top

(double) a / b
来源：http://bgo.yvedp.cn

[S16] C：位操作置位
来源：http://wef.cheryme.top

x |= (1 << 3);
来源：http://cop.ppjwa.cn

[S17] C：安全拼接字符串
来源：http://qbc.jinghuilouyu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tsn.c1oappe.top

[S18] C：命令行参数
来源：http://udu.hcnkem.com

int main(int argc, char **argv)
来源：http://rir.chenjidiqi.icu

[S19] C：快速排序
来源：http://cls.jinghuilouyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jqc.vqdsnc.cn

[S20] C：二分查找
来源：http://oms.daxiang520.top


<!-- 参考信息 -->