代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wvg.yuxming.cn

[Q52] 删除指定行
来源：http://wec.zhaomingkeji.xyz

DELETE FROM users WHERE id = 10;
来源：http://gzs.jqgufenzy.top

[Q53] 按条件删除
来源：http://erq.cheryme.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xsu.sufxvd.cn

[Q54] 清空表
来源：http://wgw.daxiang520.top

TRUNCATE TABLE logs;
来源：http://wkx.yvedp.cn

[Q55] 排名（并列占位）
来源：http://sem.yuanzhike.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wps.fanxiaobao.xyz

[Q56] 密集排名（并列不占位）
来源：http://eiu.jlsjyb.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jps.zdqjudy.top

[Q57] 行号
来源：http://ktc.vqdsnc.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://agb.fehbvm.com

[Q58] 累计求和
来源：http://fah.hywenlv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nco.shuidangran.top

[Q59] 分组内累计
来源：http://opu.fehbvm.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bea.xingfuxueyuan.xyz

[Q60] 取上一行 / 下一行
来源：http://tmq.ehwqpu.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tka.pycfn.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://byg.zhengqikj.top

[Q61] 移动平均
来源：http://kls.sufxvd.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gcj.hnxiangtu.top

[Q62] 分组占比
来源：http://asy.jqgfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://stu.yongpay.top

[Q63] 开启事务
来源：http://yzk.hnxiangtu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jqx.yfazqb.com

[Q64] 提交事务
来源：http://lpg.gotoacloud.top

COMMIT;
来源：http://egp.jianghu66.top

[Q65] 回滚事务
来源：http://xpb.fktsv.cn

ROLLBACK;
来源：http://chx.ywan-chungtsiang.top

[Q66] 行锁查询
来源：http://pku.cashguo.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://slv.xinyue.icu

[Q67] 设置隔离级别
来源：http://teu.wangshuangyany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ebx.yj202588.top

[Q68] 保存点
来源：http://pup.hnqzz.top

SAVEPOINT sp1;
来源：http://kgc.ivvv.top

ROLLBACK TO sp1;
来源：http://oqp.shanyushiyangtech.top

[Q69] 查看执行计划
来源：http://opq.wangshuangyany.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://isk.ydzc1.top

[Q70] 更新统计信息
来源：http://gya.ydjk.org.cn

ANALYZE TABLE users;
来源：http://ogf.yangfankeji.com

[Q71] 查看建表语句
来源：http://uit.chenlongwang.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cel.uphjek.com

[Q72] 查看索引
来源：http://war.cashguo.top

SHOW INDEX FROM users;
来源：http://jzi.birdmap.top

[Q73] 查看表状态
来源：http://tep.shzxlz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uya.yueranfly.top

[Q74] 强制使用索引
来源：http://pxl.zhaomingkeji.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://skk.fehbvm.com

[Q75] 日期格式化
来源：http://rrr.52xcode.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sag.quarkkingdee.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fab.fehbvm.com

[Q76] 按天统计
来源：http://ewb.fengsongda.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ndt.shuidangran.top

[Q77] 时间加减
来源：http://mbc.shangyingyoupin.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cvu.yongpay.top

[Q78] 当前时间
来源：http://vcb.fanxiaobao.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ehr.fanxiaobao.xyz

[Q79] 字符串拼接
来源：http://ysx.daria6918.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://trm.andypj.xyz

[Q80] 字符串截取
来源：http://kzm.bbcook.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tmt.hesvh.cn

[Q81] 字符串替换
来源：http://nxk.ehwqpu.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ess.shuidangran.top

[Q82] 字符长度与字节长度
来源：http://eqo.zdqjudy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ohq.mhx1999.top

[Q83] 大小写转换
来源：http://gmf.bjfxy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qjn.svipenyu.cn

[Q84] 去除首尾空格
来源：http://vau.fehbvm.com

SELECT TRIM(name) FROM users;
来源：http://xuh.andypj.xyz

[Q85] 数值取整
来源：http://kzj.redwolf501.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://byo.cashguo.top

[Q86] 读取 JSON 字段
来源：http://tij.vehdjk.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kdo.epnwcf.com

[Q87] JSON 字段做条件
来源：http://qpe.iojbl.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qku.fehbvm.com

[Q88] 行转列（条件聚合）
来源：http://qih.chenzaomai.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zqv.xziqi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ucf.ydzc1.top

[Q89] 判断表是否存在
来源：http://mfr.chenzaomai.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ycq.epnwcf.com

[Q90] 生成序号列
来源：http://zlc.shzxlz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qqc.wangdashe.top

================================================================================
来源：http://gbt.fzhhl.top

R. Bash 专题
来源：http://yzs.haohaochexian.top

================================================================================
来源：http://nfn.hfpthk.cn

[R01] shebang 与严格模式
来源：http://xwc.vehdjk.com

#!/usr/bin/env bash
来源：http://rxo.pycfn.com

set -euo pipefail
来源：http://joo.zhixingplan.top

[R02] 变量赋值与使用
来源：http://lrs.xuetiantiany.cn

name="Tom"; echo "$name"
来源：http://gyl.pycfn.com

[R03] 只读变量
来源：http://ick.xuanzx.com

readonly PI=3.14
来源：http://tfa.xinyue.icu

[R04] 位置参数
来源：http://guf.sweek.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ped.chenzaomai.com

[R05] 参数默认值
来源：http://udp.yfazqb.com

name="${1:-default}"
来源：http://ckr.yj20258.top

[R06] 判断命令是否存在
来源：http://wmp.redwolf501.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zbn.xinyue.icu

[R07] if 判断文件
来源：http://fgh.quarkkingdee.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xzw.zhiwuduotai.top

[R08] 数值比较
来源：http://mdk.jyoumei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ubv.ivvv.top

[R09] 字符串比较
来源：http://dzj.pengpengdd.cyou

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lry.pengpengdd.cyou

[R10] 正则匹配
来源：http://nzf.jqgufenzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pzf.zhengqikj.top

[R11] case 多分支
来源：http://srl.sjlbkw.cn

case "$1" in
来源：http://ckr.cdnleiting.top

start) echo "启动" ;;
来源：http://ygc.fzhhl.top

stop)  echo "停止" ;;
来源：http://mbe.ivvv.top

*)     echo "未知命令" ;;
来源：http://pjq.guannengcc.top

esac
来源：http://okj.jinqigfzy.top

[R12] for 遍历文件
来源：http://jgb.uphjek.com

for f in *.txt; do echo "$f"; done
来源：http://bij.zhixingplan.top

[R13] for 计数循环
来源：http://jjn.jinqigfzy.top

for i in {1..10}; do echo "$i"; done
来源：http://lci.quarkkingdee.top

[R14] C 风格 for
来源：http://yun.andypj.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://irx.yueranfly.top

[R15] while 逐行读文件
来源：http://pbn.fengsongda.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qks.316326.xyz

[R16] until 等待条件
来源：http://tvi.havefunace.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kkz.hongshengwenyu.top

[R17] 数组定义与取值
来源：http://cov.feifeiyinyue.top

arr=(a b c); echo "${arr[0]}"
来源：http://ulv.chenjidiqi.icu

[R18] 遍历数组
来源：http://kbu.nwbrower.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kgz.yj202588.top

[R19] 数组长度
来源：http://wxq.zhixingplan.top

echo "${#arr[@]}"
来源：http://kao.ppjwa.cn

[R20] 关联数组（字典）
来源：http://tes.mhx1999.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bnt.sufxvd.cn

[R21] 字符串长度
来源：http://kmc.chenlongwang.top

echo "${#s}"
来源：http://lvw.dashuyun.cn

[R22] 截取子串
来源：http://kfd.zycfv.cn

echo "${s:0:5}"
来源：http://ebn.sysykeji.top

[R23] 字符串替换
来源：http://lol.redwolf501.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pkr.hcnkem.com

[R24] 大小写转换
来源：http://uco.mhx1999.top

echo "${s^^}"; echo "${s,,}"
来源：http://xqw.jinqigfzy.top

[R25] 去后缀 / 去前缀
来源：http://zrg.cheryme.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ydz.sufxvd.cn

[R26] 命令替换
来源：http://zor.jiagoushi.top

now=$(date +%F); echo "$now"
来源：http://hxf.xuanzx.com

[R27] 算术展开
来源：http://qws.birdmap.top

echo $((1 + 2 * 3))
来源：http://bvr.hesvh.cn

[R28] 浮点运算
来源：http://piu.zhengqikj.top

echo "scale=2; 10/3" | bc
来源：http://ueh.wangshuangyany.cn

[R29] 定义函数
来源：http://yam.ctjpmb.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cfx.cheryme.top

[R30] 函数返回状态码
来源：http://fyc.zdqjudy.top

f() { return 0; }; f || echo "失败了"
来源：http://mgf.yuxming.cn

[R31] 局部变量
来源：http://rxb.sjlbkw.cn

f() { local x=1; echo "$x"; }
来源：http://iqs.tian-w.cn

[R32] 参数个数校验
来源：http://ckw.jiagoushi.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://whz.ybcxt.top

[R33] 捕获错误并提示行号
来源：http://vqj.cheryme.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eno.wangdashe.top

[R34] 退出时清理
来源：http://hbc.yj20258888.top

trap 'rm -f "$tmp"' EXIT
来源：http://ayt.yonumen.top

[R35] 后台执行并等待
来源：http://wtz.jianghu66.top

sleep 5 & pid=$!; wait "$pid"
来源：http://lpk.fktsv.cn

[R36] 并发执行多个任务
来源：http://dss.yj20258.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://txm.cqqwz.cn

[R37] 把输出赋给变量
来源：http://igk.feifeiyinyue.top

files=$(ls -1)
来源：http://bof.sjlbkw.cn

[R38] 管道串联
来源：http://eob.guannengcc.top

cat a.txt | grep -i error | wc -l
来源：http://toi.fehbvm.com

[R39] 重定向标准输出与错误
来源：http://dwq.yangfankeji.com

cmd > out.log 2>&1
来源：http://lmd.jianghu66.top

[R40] 追加写日志
来源：http://ztt.xuanzx.com

echo "log" >> out.log
来源：http://cot.fktsv.cn

[R41] 丢弃输出
来源：http://auu.jlsjyb.cn

cmd >/dev/null 2>&1
来源：http://eqf.zhaomingkeji.xyz

[R42] 输入重定向
来源：http://xmm.havefunace.top

wc -l < a.txt
来源：http://iwz.yfazqb.com

[R43] 按名字查找文件
来源：http://qct.hfpthk.cn

find . -name "*.log" -type f
来源：http://opw.chenjidiqi.icu

[R44] 按修改时间查找
来源：http://dpq.fktsv.cn

find . -mtime -7 -type f
来源：http://idu.meibo888.top

[R45] 批量删除
来源：http://gmo.meibo888.top

find . -name "*.tmp" -delete
来源：http://itj.hcnkem.com

[R46] 递归替换文件内容
来源：http://iud.andypj.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tbj.jinghuilouyu.cn

[R47] sed 单行替换
来源：http://qwt.gzhubu.top

sed -i 's/foo/bar/g' a.txt
来源：http://zzf.c1oappe.top

[R48] awk 取指定列
来源：http://ecl.feifeiyinyue.top

awk '{print $1, $3}' a.txt
来源：http://fhq.vqdsnc.cn

[R49] awk 带条件
来源：http://mji.hnqzz.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mqb.pycfn.com

[R50] awk 求和
来源：http://dqt.zhaomingkeji.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://hjt.hysaishi.cn

[R51] 排序去重取前几
来源：http://tip.shuidangran.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dfr.zhixingplan.top

[R52] 统计行数
来源：http://xbm.hnqzz.top

wc -l a.txt
来源：http://tvx.316326.xyz

[R53] 查看文件头与实时尾
来源：http://nqr.uphjek.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xfj.shangyingyoupin.top

[R54] 比较两个文件
来源：http://mqq.jlsjyb.cn

diff a.txt b.txt
来源：http://vok.feifeiyinyue.top

[R55] 压缩与解压
来源：http://jcw.iojbl.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hqq.shuidangran.top

[R56] 远程拷贝
来源：http://oml.havefunace.top

scp file user@host:/path/
来源：http://ydi.wangshuangyany.cn

[R57] 远程执行命令
来源：http://ocm.fengsongda.top

ssh user@host 'uptime'
来源：http://zmn.sjlbkw.cn

[R58] 下载文件
来源：http://ykn.fktsv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qyn.chenjidiqi.icu

[R59] 发 POST JSON
来源：http://zsx.zhongyouzk.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wkr.zhengqikj.top

[R60] 只看 HTTP 状态码
来源：http://sib.guannengcc.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pxb.yj20258.top

[R61] 磁盘占用
来源：http://yni.kuanghao11.cn

df -h;  du -sh *
来源：http://cyj.xylfe.cn

[R62] 找最占空间的文件
来源：http://wbk.tanke756.top

du -ah . | sort -rh | head -10
来源：http://xnm.ydzc1.top

[R63] 内存与进程
来源：http://tdv.yj202588.top

free -h;  ps aux | grep nginx
来源：http://ubh.zhoulong.xyz

[R64] 结束进程
来源：http://akx.jlsjyb.cn

kill -9 $(pgrep -f app.py)
来源：http://vpe.ydzc1.top

[R65] 查看端口占用
来源：http://qct.yvedp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://clk.chenlongwang.top

[R66] 定时任务
来源：http://oxn.ybcxt.top

crontab -e;  crontab -l
来源：http://rfl.pycfn.com

[R67] 生成随机十六进制串
来源：http://wvx.daxiang520.top

openssl rand -hex 16
来源：http://stt.birdmap.top

[R68] 计算文件校验值
来源：http://akb.havefunace.top

sha256sum a.txt;  md5sum a.txt
来源：http://fpt.52xcode.cn

[R69] 生成随机密码
来源：http://pls.xziqi.cn

head -c 16 /dev/urandom | base64
来源：http://gra.cqqwz.cn

[R70] 时间戳与互转
来源：http://zoy.chenlongwang.top

date +%s;  date -d @1700000000
来源：http://yga.mhx1999.top

[R71] 日期格式化
来源：http://vsj.yangfankeji.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://jdx.chenjidiqi.icu

[R72] 等待端口就绪
来源：http://oep.aibaodan.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pzi.jlsjyb.cn

[R73] 分割大日志
来源：http://qvo.meibo888.top

split -l 1000 big.log part_
来源：http://bdw.gogol.net.cn

[R74] 批量重命名
来源：http://zgp.xuetiantiany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rny.jlsjyb.cn

[R75] 导出环境变量
来源：http://qhy.pycfn.com

export PATH="$HOME/bin:$PATH"
来源：http://wha.xinyue.icu

[R76] 使用临时文件
来源：http://fiu.zycfv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dto.cdnleiting.top

[R77] 读取用户输入
来源：http://jqi.hesvh.cn

read -rp "请输入: " ans
来源：http://gmp.zhengqikj.top

[R78] 交互式菜单
来源：http://wfw.316326.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://wxh.shuidangran.top

[R79] 解析命令行选项
来源：http://taw.zycfv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fbo.bjfxy.top

[R80] 查看脚本执行耗时
来源：http://rsf.52xcode.cn

time ./run.sh
来源：http://dfq.fktsv.cn

================================================================================
来源：http://npw.zhiwuduotai.top

S. C / C++ 专题
来源：http://kpu.hammf.cn

================================================================================
来源：http://hbb.chenjidiqi.icu

[S01] C：Hello World
来源：http://sjq.yongpay.top

#include <stdio.h>
来源：http://jcz.gaohongyu789.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kqs.haohaochexian.top

[S02] C：变量与格式化输出
来源：http://jph.hywenlv.cn

int a = 10; printf("%d\n", a);
来源：http://src.jqgufenzy.top

[S03] C：读入整数
来源：http://wdo.c1oappe.top

int x; scanf("%d", &x);
来源：http://nxy.guowangkeji.top

[S04] C：字符串复制
来源：http://izy.sufxvd.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rzx.zhongyouzk.top

[S05] C：字符串长度
来源：http://ymx.wangshuangyany.cn

strlen(s)
来源：http://fjf.jinqigufen.top

[S06] C：字符串比较
来源：http://env.daria6918.cn

strcmp(a, b) == 0
来源：http://ndj.cheryme.top

[S07] C：数组遍历求和
来源：http://nrr.hnqzz.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://leu.jiagoushi.top

[S08] C：动态内存分配与释放
来源：http://gdw.hnxiangtu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kcb.yanxiufei.cn

[S09] C：结构体定义与初始化
来源：http://odi.epnwcf.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://azk.shzxlz.cn

[S10] C：指针与解引用
来源：http://egp.cucudq.cn

int *p = &a;  *p = 5;
来源：http://gle.pengpengdd.cyou

[S11] C：逐行读文件
来源：http://hsi.yuxming.cn

FILE *f = fopen("a.txt", "r");
来源：http://pls.bjfxy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ikd.jinyuanbaomall.cn

fclose(f);
来源：http://zgx.epnwcf.com

[S12] C：写文件
来源：http://hia.yonumen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xoc.yonumen.top

[S13] C：宏定义
来源：http://lto.fengsongda.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nla.fehbvm.com

[S14] C：枚举
来源：http://xnv.guowangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://but.xylfe.cn

[S15] C：类型转换
来源：http://mrr.jqgufenzy.top

(double) a / b
来源：http://vpc.yvedp.cn

[S16] C：位操作置位
来源：http://rtk.quarkkingdee.top

x |= (1 << 3);
来源：http://vio.hongshengwenyu.top

[S17] C：安全拼接字符串
来源：http://twc.feifeiyinyue.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qnx.jqgufenzy.top

[S18] C：命令行参数
来源：http://gjo.yj20258888.top

int main(int argc, char **argv)
来源：http://fic.gogol.net.cn

[S19] C：快速排序
来源：http://kar.nanxinkj.top

qsort(a, n, sizeof(int), cmp);
来源：http://fnl.yueranfly.top

[S20] C：二分查找
来源：http://tvh.yonumen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pvc.feifeiyinyue.top

[S21] C：字符类别判断
来源：http://dms.jlsjyb.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pgd.ybcxt.top

[S22] C：字符串转数字
来源：http://idn.wangshuangyany.cn


<!-- 参考信息 -->