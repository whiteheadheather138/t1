代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kuv.xingfuxueyuan.xyz

[Q50] 批量更新
来源：http://hbj.fktsv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qac.gzhubu.top

[Q51] 用子查询更新
来源：http://ayn.jinqigufen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lkw.xziqi.cn

[Q52] 删除指定行
来源：http://hjj.sweek.top

DELETE FROM users WHERE id = 10;
来源：http://gts.jqgufenzy.top

[Q53] 按条件删除
来源：http://meb.jinqigfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oud.daxiang520.top

[Q54] 清空表
来源：http://oiv.jinyuanbaomall.cn

TRUNCATE TABLE logs;
来源：http://lhv.shangyingyoupin.top

[Q55] 排名（并列占位）
来源：http://cwj.sysykeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mem.316326.xyz

[Q56] 密集排名（并列不占位）
来源：http://zqs.jlsjyb.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vug.pengpengdd.cyou

[Q57] 行号
来源：http://bjb.ybcxt.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eru.yj202588.top

[Q58] 累计求和
来源：http://suy.cdnleiting.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xyr.jlsjyb.cn

[Q59] 分组内累计
来源：http://irx.kuanghao11.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bhk.epnwcf.com

[Q60] 取上一行 / 下一行
来源：http://alz.yuxming.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://aaw.shangyingyoupin.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yef.zhoulong.xyz

[Q61] 移动平均
来源：http://axl.cdnleiting.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://shm.c1oappe.top

[Q62] 分组占比
来源：http://xix.aizwys.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jpv.zhixingplan.top

[Q63] 开启事务
来源：http://heo.zhengqikj.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zbd.yongpay.top

[Q64] 提交事务
来源：http://jej.shzxlz.cn

COMMIT;
来源：http://hvs.hnqzz.top

[Q65] 回滚事务
来源：http://dnb.uphjek.com

ROLLBACK;
来源：http://dzw.jinqigfzy.top

[Q66] 行锁查询
来源：http://dmw.tian-w.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qeu.cqqwz.cn

[Q67] 设置隔离级别
来源：http://jwf.yongpay.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nsy.nanxinkj.top

[Q68] 保存点
来源：http://hdv.sweek.top

SAVEPOINT sp1;
来源：http://efo.sysykeji.top

ROLLBACK TO sp1;
来源：http://mth.shangyingyoupin.top

[Q69] 查看执行计划
来源：http://hgs.yangfankeji.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hic.quarkkingdee.top

[Q70] 更新统计信息
来源：http://ntv.sufxvd.cn

ANALYZE TABLE users;
来源：http://hmn.nanxuanxn.top

[Q71] 查看建表语句
来源：http://qdb.wangshuangyany.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ivg.ctjpmb.com

[Q72] 查看索引
来源：http://uyf.gogol.net.cn

SHOW INDEX FROM users;
来源：http://ike.316326.xyz

[Q73] 查看表状态
来源：http://gbg.fzhhl.top

SHOW TABLE STATUS LIKE 'users';
来源：http://bfs.hfpthk.cn

[Q74] 强制使用索引
来源：http://exl.gogol.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gai.ivvv.top

[Q75] 日期格式化
来源：http://pls.yuxming.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vut.xuanzx.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pso.0kj1m.cn

[Q76] 按天统计
来源：http://qkb.yj20258888.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zoz.sufxvd.cn

[Q77] 时间加减
来源：http://xmd.yonumen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lbk.xuetiantiany.cn

[Q78] 当前时间
来源：http://tjm.xylfe.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wbl.ehwqpu.com

[Q79] 字符串拼接
来源：http://xcg.wangdashe.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://doe.sysykeji.top

[Q80] 字符串截取
来源：http://ewp.bbcook.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xzl.jqgufenzy.top

[Q81] 字符串替换
来源：http://haz.ywan-chungtsiang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bdh.shzxlz.cn

[Q82] 字符长度与字节长度
来源：http://wsu.yongpay.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yom.cheryme.top

[Q83] 大小写转换
来源：http://ndr.tian-w.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lfz.nanxuanxn.top

[Q84] 去除首尾空格
来源：http://lds.yj20258888.top

SELECT TRIM(name) FROM users;
来源：http://ktt.c1oappe.top

[Q85] 数值取整
来源：http://juv.gogol.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fyu.jqgfzy.top

[Q86] 读取 JSON 字段
来源：http://asf.bjfxy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dlb.dianchejie.cn

[Q87] JSON 字段做条件
来源：http://bdj.wangdashe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xta.zhoulong.xyz

[Q88] 行转列（条件聚合）
来源：http://lja.nanxinkj.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bus.chenzaomai.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jfz.sufxvd.cn

[Q89] 判断表是否存在
来源：http://lsd.cheryme.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xcl.xuanzx.com

[Q90] 生成序号列
来源：http://twl.316326.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dbz.cucudq.cn

================================================================================
来源：http://qkz.pycfn.com

R. Bash 专题
来源：http://abu.hcnkem.com

================================================================================
来源：http://jsu.sjlbkw.cn

[R01] shebang 与严格模式
来源：http://ofh.sxryk.cn

#!/usr/bin/env bash
来源：http://rpv.fktsv.cn

set -euo pipefail
来源：http://jgk.xylfe.cn

[R02] 变量赋值与使用
来源：http://yzn.gotoacloud.top

name="Tom"; echo "$name"
来源：http://ayn.uphjek.com

[R03] 只读变量
来源：http://byi.bjfxy.top

readonly PI=3.14
来源：http://sjp.vehdjk.com

[R04] 位置参数
来源：http://krl.chenlongwang.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pfe.cucudq.cn

[R05] 参数默认值
来源：http://xlr.jyoumei.cn

name="${1:-default}"
来源：http://izc.jiagoushi.top

[R06] 判断命令是否存在
来源：http://kbs.52xcode.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://von.yangfankeji.com

[R07] if 判断文件
来源：http://ccs.tian-w.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qwv.hnxiangtu.top

[R08] 数值比较
来源：http://juv.hcnkem.com

if (( a > b )); then echo "a 更大"; fi
来源：http://fok.hywenlv.cn

[R09] 字符串比较
来源：http://zyt.snrcjt.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://owq.gotoacloud.top

[R10] 正则匹配
来源：http://rdv.shanyushiyangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kns.iojbl.cn

[R11] case 多分支
来源：http://ppo.aibaodan.cn

case "$1" in
来源：http://hjc.dianchejie.cn

start) echo "启动" ;;
来源：http://kxf.zycfv.cn

stop)  echo "停止" ;;
来源：http://hyf.fehbvm.com

*)     echo "未知命令" ;;
来源：http://ele.ydjk.org.cn

esac
来源：http://nne.hammf.cn

[R12] for 遍历文件
来源：http://tmr.xziqi.cn

for f in *.txt; do echo "$f"; done
来源：http://evi.yfazqb.com

[R13] for 计数循环
来源：http://eho.haohaochexian.top

for i in {1..10}; do echo "$i"; done
来源：http://ngr.meibo888.top

[R14] C 风格 for
来源：http://soe.tarul.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pwg.sufxvd.cn

[R15] while 逐行读文件
来源：http://aaw.ydjk.org.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wtd.yj202588.top

[R16] until 等待条件
来源：http://edg.jiagoushi.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://etq.gzhubu.top

[R17] 数组定义与取值
来源：http://hmv.hcnkem.com

arr=(a b c); echo "${arr[0]}"
来源：http://orw.hysaishi.cn

[R18] 遍历数组
来源：http://uls.mhx1999.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uob.guowangkeji.top

[R19] 数组长度
来源：http://zmf.zhengqikj.top

echo "${#arr[@]}"
来源：http://ekr.zhaomingkeji.xyz

[R20] 关联数组（字典）
来源：http://vns.xuanzx.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://etl.havefunace.top

[R21] 字符串长度
来源：http://rez.ydjk.org.cn

echo "${#s}"
来源：http://aiw.hnxiangtu.top

[R22] 截取子串
来源：http://vkl.yfazqb.com

echo "${s:0:5}"
来源：http://khg.yuanzhike.top

[R23] 字符串替换
来源：http://xck.316326.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lkv.aizwys.cn

[R24] 大小写转换
来源：http://jpi.jlsjyb.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cju.yongpay.top

[R25] 去后缀 / 去前缀
来源：http://ihn.nanxinkj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://cri.tian-w.cn

[R26] 命令替换
来源：http://ygd.jinyuanbaomall.cn

now=$(date +%F); echo "$now"
来源：http://vku.xziqi.cn

[R27] 算术展开
来源：http://kig.tian-w.cn

echo $((1 + 2 * 3))
来源：http://ksw.andypj.xyz

[R28] 浮点运算
来源：http://ssq.shuidangran.top

echo "scale=2; 10/3" | bc
来源：http://bdn.316326.xyz

[R29] 定义函数
来源：http://kce.jiagoushi.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yom.jiagoushi.top

[R30] 函数返回状态码
来源：http://ram.kuanghao11.cn

f() { return 0; }; f || echo "失败了"
来源：http://gcr.zhongyouzk.top

[R31] 局部变量
来源：http://oso.fengsongda.top

f() { local x=1; echo "$x"; }
来源：http://pjq.jianghu66.top

[R32] 参数个数校验
来源：http://quw.yuanzhike.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yjb.kuanghao11.cn

[R33] 捕获错误并提示行号
来源：http://wbi.jlsjyb.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wgs.bjfxy.top

[R34] 退出时清理
来源：http://bio.fzhhl.top

trap 'rm -f "$tmp"' EXIT
来源：http://sgg.vehdjk.com

[R35] 后台执行并等待
来源：http://mvz.316326.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://qww.daria6918.cn

[R36] 并发执行多个任务
来源：http://agn.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://exp.wangdashe.top

[R37] 把输出赋给变量
来源：http://ige.ywan-chungtsiang.top

files=$(ls -1)
来源：http://gjk.jqgfzy.top

[R38] 管道串联
来源：http://tky.zdbjq.cn

cat a.txt | grep -i error | wc -l
来源：http://wcr.sufxvd.cn

[R39] 重定向标准输出与错误
来源：http://yzl.tian-w.cn

cmd > out.log 2>&1
来源：http://mvv.zhongyouzk.top

[R40] 追加写日志
来源：http://dfb.pengpengdd.cyou

echo "log" >> out.log
来源：http://fbo.yonumen.top

[R41] 丢弃输出
来源：http://fir.gogol.net.cn

cmd >/dev/null 2>&1
来源：http://vrr.jinqigufen.top

[R42] 输入重定向
来源：http://mzj.jinqigfzy.top

wc -l < a.txt
来源：http://caw.c1oappe.top

[R43] 按名字查找文件
来源：http://ftv.jqgufenzy.top

find . -name "*.log" -type f
来源：http://viz.quarkkingdee.top

[R44] 按修改时间查找
来源：http://ack.nanxinkj.top

find . -mtime -7 -type f
来源：http://zgp.zhengqikj.top

[R45] 批量删除
来源：http://rrc.jiagoushi.top

find . -name "*.tmp" -delete
来源：http://raf.daria6918.cn

[R46] 递归替换文件内容
来源：http://umf.chenjidiqi.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pwn.jyoumei.cn

[R47] sed 单行替换
来源：http://ths.yj20258888.top

sed -i 's/foo/bar/g' a.txt
来源：http://ttp.xinyue.icu

[R48] awk 取指定列
来源：http://twl.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://rvx.yangfankeji.com

[R49] awk 带条件
来源：http://kpy.fanxiaobao.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dia.zdqjudy.top

[R50] awk 求和
来源：http://rcr.daria6918.cn

awk '{s += $2} END {print s}' a.txt
来源：http://agx.shangyingyoupin.top

[R51] 排序去重取前几
来源：http://nvk.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xgf.hnqzz.top

[R52] 统计行数
来源：http://hzw.hcnkem.com

wc -l a.txt
来源：http://hxe.hysaishi.cn

[R53] 查看文件头与实时尾
来源：http://rvz.ywan-chungtsiang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tlx.guowangkeji.top

[R54] 比较两个文件
来源：http://hjg.uphjek.com

diff a.txt b.txt
来源：http://fgp.uphjek.com

[R55] 压缩与解压
来源：http://vvh.jiagoushi.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://brn.gzhubu.top

[R56] 远程拷贝
来源：http://zse.shanyushiyangkeji.top

scp file user@host:/path/
来源：http://mmj.shuidangran.top

[R57] 远程执行命令
来源：http://plo.sufxvd.cn

ssh user@host 'uptime'
来源：http://duq.zhiwuduotai.top

[R58] 下载文件
来源：http://vsy.hfpthk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://aev.zhiwuduotai.top

[R59] 发 POST JSON
来源：http://ldd.jinqigufen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://phc.xylfe.cn

[R60] 只看 HTTP 状态码
来源：http://foq.sweek.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mod.chenjidiqi.icu

[R61] 磁盘占用
来源：http://kna.shuidangran.top

df -h;  du -sh *
来源：http://qwy.yj20258888.top

[R62] 找最占空间的文件
来源：http://bow.9152youxi.cn

du -ah . | sort -rh | head -10
来源：http://jer.vqdsnc.cn

[R63] 内存与进程
来源：http://xos.andypj.xyz

free -h;  ps aux | grep nginx
来源：http://ppm.dashuyun.cn

[R64] 结束进程
来源：http://fnz.jinqigufen.top

kill -9 $(pgrep -f app.py)
来源：http://afg.tianlin.xyz

[R65] 查看端口占用
来源：http://fuh.chenlongwang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zwj.hfpthk.cn

[R66] 定时任务
来源：http://xdc.ydjk.org.cn

crontab -e;  crontab -l
来源：http://yve.fktsv.cn

[R67] 生成随机十六进制串
来源：http://eln.zhixingplan.top

openssl rand -hex 16
来源：http://cix.daxiang520.top

[R68] 计算文件校验值
来源：http://qxq.0kj1m.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zpe.wangshuangyany.cn

[R69] 生成随机密码
来源：http://ndn.fzhhl.top

head -c 16 /dev/urandom | base64
来源：http://tcy.sysykeji.top

[R70] 时间戳与互转
来源：http://gjl.sweek.top

date +%s;  date -d @1700000000
来源：http://wtf.feifeiyinyue.top

[R71] 日期格式化
来源：http://qwx.jyoumei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://eck.bbcook.cn

[R72] 等待端口就绪
来源：http://vli.fzhhl.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ivo.jiagoushi.top

[R73] 分割大日志
来源：http://tme.zhaomingkeji.xyz

split -l 1000 big.log part_
来源：http://xgd.aibaodan.cn

[R74] 批量重命名
来源：http://swk.hongshengwenyu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vgr.jlsjyb.cn

[R75] 导出环境变量
来源：http://mnn.epnwcf.com

export PATH="$HOME/bin:$PATH"
来源：http://fon.zhongyouzk.top

[R76] 使用临时文件
来源：http://epc.vehdjk.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ugn.9152youxi.cn

[R77] 读取用户输入
来源：http://cjp.epnwcf.com

read -rp "请输入: " ans
来源：http://ueg.cheryme.top

[R78] 交互式菜单
来源：http://ktk.fehbvm.com

select opt in a b c; do echo "$opt"; break; done
来源：http://hod.zhiwuduotai.top

[R79] 解析命令行选项
来源：http://bsv.dashuyun.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mts.zdbjq.cn

[R80] 查看脚本执行耗时
来源：http://tva.jqgufenzy.top

time ./run.sh
来源：http://bze.hfpthk.cn

================================================================================
来源：http://eaf.hnqzz.top

S. C / C++ 专题
来源：http://ryj.ybcxt.top

================================================================================
来源：http://xpc.vehdjk.com

[S01] C：Hello World
来源：http://zcc.zhongyouzk.top

#include <stdio.h>
来源：http://bdn.jinqigfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://tjj.yj20258888.top

[S02] C：变量与格式化输出
来源：http://uic.yfazqb.com

int a = 10; printf("%d\n", a);
来源：http://oxt.316326.xyz

[S03] C：读入整数
来源：http://gnw.ydzc1.top

int x; scanf("%d", &x);
来源：http://cek.hongshengwenyu.top

[S04] C：字符串复制
来源：http://fel.chenlongwang.top

char dst[32]; strcpy(dst, "hi");
来源：http://zdm.pengpengdd.cyou

[S05] C：字符串长度
来源：http://yzu.mhx1999.top

strlen(s)
来源：http://acf.c1oappe.top

[S06] C：字符串比较
来源：http://lmt.hcnkem.com

strcmp(a, b) == 0
来源：http://hdk.yonumen.top

[S07] C：数组遍历求和
来源：http://ztf.shzxlz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ulq.birdmap.top

[S08] C：动态内存分配与释放
来源：http://nyo.hywenlv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lkj.fzhhl.top

[S09] C：结构体定义与初始化
来源：http://ipq.xinyue.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nnb.zhengqikj.top

[S10] C：指针与解引用
来源：http://xyk.hongshengwenyu.top

int *p = &a;  *p = 5;
来源：http://gpz.sufxvd.cn

[S11] C：逐行读文件
来源：http://sjg.ydjk.org.cn

FILE *f = fopen("a.txt", "r");
来源：http://esu.cucudq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nyk.sweek.top

fclose(f);
来源：http://bef.ivvv.top

[S12] C：写文件
来源：http://izo.aizwys.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://grz.xuetiantiany.cn

[S13] C：宏定义
来源：http://azk.yj202588.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dbn.cheryme.top

[S14] C：枚举
来源：http://kxp.shanyushiyangtech.top

enum Color { RED, GREEN, BLUE };
来源：http://fxt.yongpay.top

[S15] C：类型转换
来源：http://tea.bjfxy.top

(double) a / b
来源：http://vab.zhijiandao.cn

[S16] C：位操作置位
来源：http://lbz.bbcook.cn

x |= (1 << 3);
来源：http://eox.jqgfzy.top

[S17] C：安全拼接字符串
来源：http://hwg.zhaomingkeji.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wsp.birdmap.top

[S18] C：命令行参数
来源：http://aiq.epnwcf.com

int main(int argc, char **argv)
来源：http://kim.redwolf501.top

[S19] C：快速排序
来源：http://dpc.guowangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://wud.chenzaomai.com

[S20] C：二分查找
来源：http://jhu.yongpay.top


<!-- 参考信息 -->