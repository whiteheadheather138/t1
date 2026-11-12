代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qyq.bbcook.cn

[Q56] 密集排名（并列不占位）
来源：http://kkj.guannengcc.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cem.jiagoushi.top

[Q57] 行号
来源：http://cbv.iojbl.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mjy.yuxming.cn

[Q58] 累计求和
来源：http://npw.xylfe.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://afb.wangdashe.top

[Q59] 分组内累计
来源：http://qge.bjfxy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cyf.cheryme.top

[Q60] 取上一行 / 下一行
来源：http://arb.ybcxt.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mcq.tanke756.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rjd.shangyingyoupin.top

[Q61] 移动平均
来源：http://gex.kuanghao11.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jll.shangyingyoupin.top

[Q62] 分组占比
来源：http://ojl.hfpthk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vtp.fktsv.cn

[Q63] 开启事务
来源：http://etq.xuanzx.com

START TRANSACTION;                -- 或 BEGIN
来源：http://vpp.xziqi.cn

[Q64] 提交事务
来源：http://lzv.tian-w.cn

COMMIT;
来源：http://jkj.wangshuangyany.cn

[Q65] 回滚事务
来源：http://kvz.xuetiantiany.cn

ROLLBACK;
来源：http://euo.xingfuxueyuan.xyz

[Q66] 行锁查询
来源：http://fwu.c1oappe.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kyd.tian-w.cn

[Q67] 设置隔离级别
来源：http://cxl.uphjek.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://utj.gotoacloud.top

[Q68] 保存点
来源：http://qsm.yvedp.cn

SAVEPOINT sp1;
来源：http://mgx.fehbvm.com

ROLLBACK TO sp1;
来源：http://sks.ppjwa.cn

[Q69] 查看执行计划
来源：http://cba.yuxming.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fdd.gzhubu.top

[Q70] 更新统计信息
来源：http://wkp.sufxvd.cn

ANALYZE TABLE users;
来源：http://vjz.fzhhl.top

[Q71] 查看建表语句
来源：http://tub.ybcxt.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xmv.jianghu66.top

[Q72] 查看索引
来源：http://fhn.guowangkeji.top

SHOW INDEX FROM users;
来源：http://owr.guowangkeji.top

[Q73] 查看表状态
来源：http://ujy.dashuyun.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rym.fehbvm.com

[Q74] 强制使用索引
来源：http://jzo.9152youxi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mup.zdbjq.cn

[Q75] 日期格式化
来源：http://xfa.svipenyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jhv.ctjpmb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zwm.ydzc1.top

[Q76] 按天统计
来源：http://stj.hfpthk.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yri.nanxinkj.top

[Q77] 时间加减
来源：http://eyp.guannengcc.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://htt.mhx1999.top

[Q78] 当前时间
来源：http://tha.nanxuanxn.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lkw.c1oappe.top

[Q79] 字符串拼接
来源：http://bqw.nwbrower.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://psk.snrcjt.cn

[Q80] 字符串截取
来源：http://acg.dashuyun.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lej.daxiang520.top

[Q81] 字符串替换
来源：http://tif.wangshuangyany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xbz.ivvv.top

[Q82] 字符长度与字节长度
来源：http://zfm.jqgufenzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yjd.sweek.top

[Q83] 大小写转换
来源：http://guv.jinqigfzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mrd.shangyingyoupin.top

[Q84] 去除首尾空格
来源：http://dke.zhengqikj.top

SELECT TRIM(name) FROM users;
来源：http://wtu.aibaodan.cn

[Q85] 数值取整
来源：http://tkq.hysaishi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cfc.kuanghao11.cn

[Q86] 读取 JSON 字段
来源：http://epr.gotoacloud.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tpf.nanxinkj.top

[Q87] JSON 字段做条件
来源：http://vry.tian-w.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lxu.bbcook.cn

[Q88] 行转列（条件聚合）
来源：http://hrr.tanke756.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gxm.yueranfly.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rie.gaohongyu789.top

[Q89] 判断表是否存在
来源：http://igb.pengpengdd.cyou

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cut.havefunace.top

[Q90] 生成序号列
来源：http://iyy.tanke756.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wyu.ywan-chungtsiang.top

================================================================================
来源：http://scj.andypj.xyz

R. Bash 专题
来源：http://ocb.chenzaomai.com

================================================================================
来源：http://lhb.zhijiandao.cn

[R01] shebang 与严格模式
来源：http://avl.cqqwz.cn

#!/usr/bin/env bash
来源：http://ooj.sysykeji.top

set -euo pipefail
来源：http://coh.snrcjt.cn

[R02] 变量赋值与使用
来源：http://jop.xylfe.cn

name="Tom"; echo "$name"
来源：http://sup.jiagoushi.top

[R03] 只读变量
来源：http://kjx.ctjpmb.com

readonly PI=3.14
来源：http://hko.smart0.xyz

[R04] 位置参数
来源：http://kge.hammf.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nje.uphjek.com

[R05] 参数默认值
来源：http://fsi.jlsjyb.cn

name="${1:-default}"
来源：http://neh.epnwcf.com

[R06] 判断命令是否存在
来源：http://lhm.fengsongda.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yaa.dashuyun.cn

[R07] if 判断文件
来源：http://xpd.yonumen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cpr.zdbjq.cn

[R08] 数值比较
来源：http://uvl.ydzc1.top

if (( a > b )); then echo "a 更大"; fi
来源：http://hkp.epnwcf.com

[R09] 字符串比较
来源：http://psm.ywan-chungtsiang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://npg.ybcxt.top

[R10] 正则匹配
来源：http://mip.snrcjt.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bmg.fktsv.cn

[R11] case 多分支
来源：http://vxb.cucudq.cn

case "$1" in
来源：http://fqe.fktsv.cn

start) echo "启动" ;;
来源：http://yql.yongpay.top

stop)  echo "停止" ;;
来源：http://jwt.shanyushiyangtech.top

*)     echo "未知命令" ;;
来源：http://xln.yangfankeji.com

esac
来源：http://flr.guannengcc.top

[R12] for 遍历文件
来源：http://mdn.fengsongda.top

for f in *.txt; do echo "$f"; done
来源：http://zcy.fanxiaobao.xyz

[R13] for 计数循环
来源：http://idi.xingfuxueyuan.xyz

for i in {1..10}; do echo "$i"; done
来源：http://xlc.0kj1m.cn

[R14] C 风格 for
来源：http://mhl.iojbl.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tmn.sweek.top

[R15] while 逐行读文件
来源：http://pvk.ydjk.org.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nzd.snrcjt.cn

[R16] until 等待条件
来源：http://qqq.chenlongwang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ldw.zdbjq.cn

[R17] 数组定义与取值
来源：http://kmm.hysaishi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cwj.hongshengwenyu.top

[R18] 遍历数组
来源：http://zys.zhengqikj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pvh.sweek.top

[R19] 数组长度
来源：http://iph.xziqi.cn

echo "${#arr[@]}"
来源：http://kxe.ydzc1.top

[R20] 关联数组（字典）
来源：http://hrf.epnwcf.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hag.wangdashe.top

[R21] 字符串长度
来源：http://gsy.hnqzz.top

echo "${#s}"
来源：http://jqs.pycfn.com

[R22] 截取子串
来源：http://jey.yj202588.top

echo "${s:0:5}"
来源：http://xwi.yuanzhike.top

[R23] 字符串替换
来源：http://ret.yuxming.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ace.yj202588.top

[R24] 大小写转换
来源：http://otb.fengsongda.top

echo "${s^^}"; echo "${s,,}"
来源：http://aib.kuanghao11.cn

[R25] 去后缀 / 去前缀
来源：http://hwz.gzhubu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://foe.yuxming.cn

[R26] 命令替换
来源：http://nnq.meibo888.top

now=$(date +%F); echo "$now"
来源：http://ula.birdmap.top

[R27] 算术展开
来源：http://niy.daxiang520.top

echo $((1 + 2 * 3))
来源：http://qwb.jqgfzy.top

[R28] 浮点运算
来源：http://ube.dianchejie.cn

echo "scale=2; 10/3" | bc
来源：http://ncy.jinyuanbaomall.cn

[R29] 定义函数
来源：http://myq.zhixingplan.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wft.c1oappe.top

[R30] 函数返回状态码
来源：http://ixt.chenjidiqi.icu

f() { return 0; }; f || echo "失败了"
来源：http://tbp.hnqzz.top

[R31] 局部变量
来源：http://sgj.sufxvd.cn

f() { local x=1; echo "$x"; }
来源：http://dws.cheryme.top

[R32] 参数个数校验
来源：http://jxh.haohaochexian.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oco.sxryk.cn

[R33] 捕获错误并提示行号
来源：http://qqm.aizwys.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://onu.hongshengwenyu.top

[R34] 退出时清理
来源：http://lhc.ppjwa.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cvo.mhx1999.top

[R35] 后台执行并等待
来源：http://apk.tian-w.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hzv.sufxvd.cn

[R36] 并发执行多个任务
来源：http://rtr.daria6918.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xda.ivvv.top

[R37] 把输出赋给变量
来源：http://ouu.zdbjq.cn

files=$(ls -1)
来源：http://ayl.yuxming.cn

[R38] 管道串联
来源：http://pyc.316326.xyz

cat a.txt | grep -i error | wc -l
来源：http://vno.hysaishi.cn

[R39] 重定向标准输出与错误
来源：http://kdg.jqgufenzy.top

cmd > out.log 2>&1
来源：http://kfr.vqdsnc.cn

[R40] 追加写日志
来源：http://djr.zhongyouzk.top

echo "log" >> out.log
来源：http://zun.nanxuanxn.top

[R41] 丢弃输出
来源：http://lgw.zhoulong.xyz

cmd >/dev/null 2>&1
来源：http://hbq.sxryk.cn

[R42] 输入重定向
来源：http://awm.pengpengdd.cyou

wc -l < a.txt
来源：http://xso.ydjk.org.cn

[R43] 按名字查找文件
来源：http://ewj.ydzc1.top

find . -name "*.log" -type f
来源：http://wgk.shzxlz.cn

[R44] 按修改时间查找
来源：http://spk.0kj1m.cn

find . -mtime -7 -type f
来源：http://udp.dashuyun.cn

[R45] 批量删除
来源：http://krs.hongshengwenyu.top

find . -name "*.tmp" -delete
来源：http://ijn.hnxiangtu.top

[R46] 递归替换文件内容
来源：http://ebj.yueranfly.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://urm.xuanzx.com

[R47] sed 单行替换
来源：http://xww.jinyuanbaomall.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dfh.zycfv.cn

[R48] awk 取指定列
来源：http://chs.jinqigfzy.top

awk '{print $1, $3}' a.txt
来源：http://awj.andypj.xyz

[R49] awk 带条件
来源：http://xcc.zhoulong.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mie.jianghu66.top

[R50] awk 求和
来源：http://fjg.svipenyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rfe.9152youxi.cn

[R51] 排序去重取前几
来源：http://pso.vehdjk.com

sort a.txt | uniq -c | sort -rn | head
来源：http://jtq.yonumen.top

[R52] 统计行数
来源：http://jnl.hywenlv.cn

wc -l a.txt
来源：http://gwi.iojbl.cn

[R53] 查看文件头与实时尾
来源：http://dzj.shzxlz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ebj.hesvh.cn

[R54] 比较两个文件
来源：http://adu.aibaodan.cn

diff a.txt b.txt
来源：http://zca.cqqwz.cn

[R55] 压缩与解压
来源：http://wyk.snrcjt.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dks.zhaomingkeji.xyz

[R56] 远程拷贝
来源：http://dfw.cqqwz.cn

scp file user@host:/path/
来源：http://kjd.svipenyu.cn

[R57] 远程执行命令
来源：http://hrc.gogol.net.cn

ssh user@host 'uptime'
来源：http://fry.guannengcc.top

[R58] 下载文件
来源：http://wyo.jinqigufen.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mcp.tanke756.top

[R59] 发 POST JSON
来源：http://del.yanxiufei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xka.cqqwz.cn

[R60] 只看 HTTP 状态码
来源：http://znr.iojbl.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ivq.wangshuangyany.cn

[R61] 磁盘占用
来源：http://xxe.316326.xyz

df -h;  du -sh *
来源：http://vmg.zhiwuduotai.top

[R62] 找最占空间的文件
来源：http://btb.c1oappe.top

du -ah . | sort -rh | head -10
来源：http://qpj.birdmap.top

[R63] 内存与进程
来源：http://ytg.zhijiandao.cn

free -h;  ps aux | grep nginx
来源：http://rxg.havefunace.top

[R64] 结束进程
来源：http://oht.xuanzx.com

kill -9 $(pgrep -f app.py)
来源：http://ngj.dianchejie.cn

[R65] 查看端口占用
来源：http://gii.hnxiangtu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dcw.nanxuanxn.top

[R66] 定时任务
来源：http://agz.shanyushiyangkeji.top

crontab -e;  crontab -l
来源：http://ixf.zdqjudy.top

[R67] 生成随机十六进制串
来源：http://qha.pengpengdd.cyou

openssl rand -hex 16
来源：http://jte.jyoumei.cn

[R68] 计算文件校验值
来源：http://gwk.bjfxy.top

sha256sum a.txt;  md5sum a.txt
来源：http://oow.hammf.cn

[R69] 生成随机密码
来源：http://epz.haohaochexian.top

head -c 16 /dev/urandom | base64
来源：http://yyx.tian-w.cn

[R70] 时间戳与互转
来源：http://ykq.chenlongwang.top

date +%s;  date -d @1700000000
来源：http://qjy.jyoumei.cn

[R71] 日期格式化
来源：http://oks.gotoacloud.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://arm.yuanzhike.top

[R72] 等待端口就绪
来源：http://txc.gzhubu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://yhw.jqgufenzy.top

[R73] 分割大日志
来源：http://xdc.hnqzz.top

split -l 1000 big.log part_
来源：http://xme.yj20258.top

[R74] 批量重命名
来源：http://psj.epnwcf.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://exd.jinyuanbaomall.cn

[R75] 导出环境变量
来源：http://wki.ivvv.top

export PATH="$HOME/bin:$PATH"
来源：http://qbw.yanxiufei.cn

[R76] 使用临时文件
来源：http://htd.hcnkem.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vll.cdnleiting.top

[R77] 读取用户输入
来源：http://qqh.ydjk.org.cn

read -rp "请输入: " ans
来源：http://wlq.hnxiangtu.top

[R78] 交互式菜单
来源：http://nic.shangyingyoupin.top

select opt in a b c; do echo "$opt"; break; done
来源：http://bym.cheryme.top

[R79] 解析命令行选项
来源：http://mbp.ywan-chungtsiang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bht.shuidangran.top

[R80] 查看脚本执行耗时
来源：http://llq.gaohongyu789.top

time ./run.sh
来源：http://smq.hysaishi.cn

================================================================================
来源：http://ibb.zdbjq.cn

S. C / C++ 专题
来源：http://xcr.shanyushiyangkeji.top

================================================================================
来源：http://oaa.jqgfzy.top

[S01] C：Hello World
来源：http://kjd.zhixingplan.top

#include <stdio.h>
来源：http://zmz.nanxuanxn.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://pug.jqgfzy.top

[S02] C：变量与格式化输出
来源：http://bly.cdnleiting.top

int a = 10; printf("%d\n", a);
来源：http://qot.yuanzhike.top

[S03] C：读入整数
来源：http://jnr.svipenyu.cn

int x; scanf("%d", &x);
来源：http://rij.9152youxi.cn

[S04] C：字符串复制
来源：http://yfc.aibaodan.cn

char dst[32]; strcpy(dst, "hi");
来源：http://twn.ivvv.top

[S05] C：字符串长度
来源：http://sis.zycfv.cn

strlen(s)
来源：http://xjq.nanxuanxn.top

[S06] C：字符串比较
来源：http://qcf.cdnleiting.top

strcmp(a, b) == 0
来源：http://lhv.zhengqikj.top

[S07] C：数组遍历求和
来源：http://kid.yuxming.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rrc.jinqigfzy.top

[S08] C：动态内存分配与释放
来源：http://fqm.xingfuxueyuan.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://asr.svipenyu.cn

[S09] C：结构体定义与初始化
来源：http://gjc.redwolf501.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bpg.cdnleiting.top

[S10] C：指针与解引用
来源：http://jmq.uphjek.com

int *p = &a;  *p = 5;
来源：http://jzf.tarul.cn

[S11] C：逐行读文件
来源：http://qbh.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://xbu.chenlongwang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://swc.daxiang520.top

fclose(f);
来源：http://fxi.zdbjq.cn

[S12] C：写文件
来源：http://ogj.hongshengwenyu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zzv.zycfv.cn

[S13] C：宏定义
来源：http://sri.daria6918.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dxj.vehdjk.com

[S14] C：枚举
来源：http://vxj.kuanghao11.cn

enum Color { RED, GREEN, BLUE };
来源：http://old.zhijiandao.cn

[S15] C：类型转换
来源：http://uog.52xcode.cn

(double) a / b
来源：http://ift.wangshuangyany.cn

[S16] C：位操作置位
来源：http://zgx.iojbl.cn

x |= (1 << 3);
来源：http://biu.bbcook.cn

[S17] C：安全拼接字符串
来源：http://gss.shuidangran.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hyc.shanyushiyangtech.top

[S18] C：命令行参数
来源：http://aon.smart0.xyz

int main(int argc, char **argv)
来源：http://xrc.xingfuxueyuan.xyz

[S19] C：快速排序
来源：http://eij.fzhhl.top

qsort(a, n, sizeof(int), cmp);
来源：http://dic.sjlbkw.cn

[S20] C：二分查找
来源：http://asj.jinqigfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yxg.gotoacloud.top

[S21] C：字符类别判断
来源：http://fpx.fengsongda.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://olm.tian-w.cn

[S22] C：字符串转数字
来源：http://pla.daria6918.cn

atoi("42");  strtod("3.14", NULL);
来源：http://blt.xylfe.cn

[S23] C：随机数
来源：http://jyg.9152youxi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yrj.daria6918.cn

[S24] C：获取本地时间
来源：http://ltb.jinqigufen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://boj.yj20258.top

[S25] C：内存拷贝
来源：http://aht.xziqi.cn

memcpy(dst, src, n);
来源：http://sit.jqgufenzy.top

[S26] C：内存清零
来源：http://yax.hesvh.cn


<!-- 参考信息 -->