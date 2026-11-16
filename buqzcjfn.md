代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fqu.xinyue.icu

[Q58] 累计求和
来源：http://zle.hysaishi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://icl.gogol.net.cn

[Q59] 分组内累计
来源：http://gql.shangyingyoupin.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wfu.zhiwuduotai.top

[Q60] 取上一行 / 下一行
来源：http://kce.sufxvd.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://iga.dianchejie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://llb.chenzaomai.com

[Q61] 移动平均
来源：http://bfo.zhijiandao.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dfp.yuanzhike.top

[Q62] 分组占比
来源：http://cul.nanxuanxn.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bej.bjfxy.top

[Q63] 开启事务
来源：http://zjr.hongshengwenyu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vdw.svipenyu.cn

[Q64] 提交事务
来源：http://wlk.yj20258.top

COMMIT;
来源：http://uwn.hammf.cn

[Q65] 回滚事务
来源：http://wxm.pycfn.com

ROLLBACK;
来源：http://ini.yj202588.top

[Q66] 行锁查询
来源：http://wgo.uphjek.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jie.xingfuxueyuan.xyz

[Q67] 设置隔离级别
来源：http://ofu.gogol.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ztr.aibaodan.cn

[Q68] 保存点
来源：http://ndn.shzxlz.cn

SAVEPOINT sp1;
来源：http://bag.zdbjq.cn

ROLLBACK TO sp1;
来源：http://sfl.jinqigufen.top

[Q69] 查看执行计划
来源：http://gsi.hysaishi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pjd.zhixingplan.top

[Q70] 更新统计信息
来源：http://qsy.svipenyu.cn

ANALYZE TABLE users;
来源：http://ogm.snrcjt.cn

[Q71] 查看建表语句
来源：http://wrs.uphjek.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lwm.gotoacloud.top

[Q72] 查看索引
来源：http://bjp.shanyushiyangkeji.top

SHOW INDEX FROM users;
来源：http://zny.gogol.net.cn

[Q73] 查看表状态
来源：http://cpl.havefunace.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wmg.nanxuanxn.top

[Q74] 强制使用索引
来源：http://afc.yonumen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zot.ivvv.top

[Q75] 日期格式化
来源：http://lif.jinghuilouyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dmg.ybcxt.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zch.jqgfzy.top

[Q76] 按天统计
来源：http://wzs.0kj1m.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ohf.fanxiaobao.xyz

[Q77] 时间加减
来源：http://cjy.cashguo.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yde.0kj1m.cn

[Q78] 当前时间
来源：http://ukl.xingfuxueyuan.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://upe.daxiang520.top

[Q79] 字符串拼接
来源：http://uvt.jqgfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qhl.nanxinkj.top

[Q80] 字符串截取
来源：http://sgo.xingfuxueyuan.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eax.vqdsnc.cn

[Q81] 字符串替换
来源：http://oyw.yuanzhike.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hgs.sxryk.cn

[Q82] 字符长度与字节长度
来源：http://wfd.tian-w.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kpn.chenjidiqi.icu

[Q83] 大小写转换
来源：http://cah.xinyue.icu

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zac.snrcjt.cn

[Q84] 去除首尾空格
来源：http://jbe.jianghu66.top

SELECT TRIM(name) FROM users;
来源：http://eqz.ivvv.top

[Q85] 数值取整
来源：http://mss.xuanzx.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fcx.9152youxi.cn

[Q86] 读取 JSON 字段
来源：http://ddl.andypj.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xou.fzhhl.top

[Q87] JSON 字段做条件
来源：http://pst.9152youxi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zzn.ywan-chungtsiang.top

[Q88] 行转列（条件聚合）
来源：http://obp.vqdsnc.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cxz.vqdsnc.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zxc.52xcode.cn

[Q89] 判断表是否存在
来源：http://kmd.ivvv.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://owe.tanke756.top

[Q90] 生成序号列
来源：http://hlq.yongpay.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bxd.jiagoushi.top

================================================================================
来源：http://rqy.iojbl.cn

R. Bash 专题
来源：http://ewq.shuidangran.top

================================================================================
来源：http://iti.jqgufenzy.top

[R01] shebang 与严格模式
来源：http://ist.yj20258.top

#!/usr/bin/env bash
来源：http://hat.bjfxy.top

set -euo pipefail
来源：http://koh.gaohongyu789.top

[R02] 变量赋值与使用
来源：http://isx.xziqi.cn

name="Tom"; echo "$name"
来源：http://xda.guannengcc.top

[R03] 只读变量
来源：http://uwe.birdmap.top

readonly PI=3.14
来源：http://rqu.yangfankeji.com

[R04] 位置参数
来源：http://xia.zycfv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qqw.feifeiyinyue.top

[R05] 参数默认值
来源：http://xty.dianchejie.cn

name="${1:-default}"
来源：http://nke.feifeiyinyue.top

[R06] 判断命令是否存在
来源：http://mcf.fehbvm.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dws.shanyushiyangtech.top

[R07] if 判断文件
来源：http://zqx.gaohongyu789.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wsm.ydzc1.top

[R08] 数值比较
来源：http://flr.xylfe.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cet.tian-w.cn

[R09] 字符串比较
来源：http://unt.fanxiaobao.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tfg.52xcode.cn

[R10] 正则匹配
来源：http://oew.hesvh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sxw.nwbrower.top

[R11] case 多分支
来源：http://fxn.cqqwz.cn

case "$1" in
来源：http://jhj.sjlbkw.cn

start) echo "启动" ;;
来源：http://zdl.chenlongwang.top

stop)  echo "停止" ;;
来源：http://snd.dashuyun.cn

*)     echo "未知命令" ;;
来源：http://evv.yfazqb.com

esac
来源：http://bzw.hnxiangtu.top

[R12] for 遍历文件
来源：http://wew.shanyushiyangtech.top

for f in *.txt; do echo "$f"; done
来源：http://vxt.vehdjk.com

[R13] for 计数循环
来源：http://qpw.yuanzhike.top

for i in {1..10}; do echo "$i"; done
来源：http://due.epnwcf.com

[R14] C 风格 for
来源：http://eoz.havefunace.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sba.yj202588.top

[R15] while 逐行读文件
来源：http://jjd.feifeiyinyue.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://euz.pengpengdd.cyou

[R16] until 等待条件
来源：http://yhz.hongshengwenyu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kqc.xuanzx.com

[R17] 数组定义与取值
来源：http://ego.hywenlv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hbz.fengsongda.top

[R18] 遍历数组
来源：http://zyp.snrcjt.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cgi.zhijiandao.cn

[R19] 数组长度
来源：http://ccn.ppjwa.cn

echo "${#arr[@]}"
来源：http://mxr.snrcjt.cn

[R20] 关联数组（字典）
来源：http://uzh.zycfv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pkd.tian-w.cn

[R21] 字符串长度
来源：http://vfx.yvedp.cn

echo "${#s}"
来源：http://ogs.ybcxt.top

[R22] 截取子串
来源：http://unr.dianchejie.cn

echo "${s:0:5}"
来源：http://nzs.hysaishi.cn

[R23] 字符串替换
来源：http://pjk.tianlin.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cdl.cucudq.cn

[R24] 大小写转换
来源：http://pmy.fengsongda.top

echo "${s^^}"; echo "${s,,}"
来源：http://kln.vqdsnc.cn

[R25] 去后缀 / 去前缀
来源：http://bah.sysykeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ibi.cqqwz.cn

[R26] 命令替换
来源：http://wzh.hammf.cn

now=$(date +%F); echo "$now"
来源：http://idi.shanyushiyangtech.top

[R27] 算术展开
来源：http://nfx.zhiwuduotai.top

echo $((1 + 2 * 3))
来源：http://ggr.cqqwz.cn

[R28] 浮点运算
来源：http://ftc.dianchejie.cn

echo "scale=2; 10/3" | bc
来源：http://oet.bbcook.cn

[R29] 定义函数
来源：http://neq.zhiwuduotai.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bfl.nwbrower.top

[R30] 函数返回状态码
来源：http://til.yueranfly.top

f() { return 0; }; f || echo "失败了"
来源：http://qjd.cdnleiting.top

[R31] 局部变量
来源：http://dkz.fktsv.cn

f() { local x=1; echo "$x"; }
来源：http://yjz.hongshengwenyu.top

[R32] 参数个数校验
来源：http://vmb.guannengcc.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fky.zhengqikj.top

[R33] 捕获错误并提示行号
来源：http://dnf.nanxinkj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tft.yuxming.cn

[R34] 退出时清理
来源：http://jcp.nanxinkj.top

trap 'rm -f "$tmp"' EXIT
来源：http://qjx.xylfe.cn

[R35] 后台执行并等待
来源：http://tjc.cashguo.top

sleep 5 & pid=$!; wait "$pid"
来源：http://qkl.mhx1999.top

[R36] 并发执行多个任务
来源：http://oph.zhijiandao.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oqi.yuanzhike.top

[R37] 把输出赋给变量
来源：http://lpa.chenlongwang.top

files=$(ls -1)
来源：http://ouh.nanxinkj.top

[R38] 管道串联
来源：http://gyi.jianghu66.top

cat a.txt | grep -i error | wc -l
来源：http://zlk.jinqigufen.top

[R39] 重定向标准输出与错误
来源：http://pgq.hongshengwenyu.top

cmd > out.log 2>&1
来源：http://kjt.jinqigufen.top

[R40] 追加写日志
来源：http://guo.hysaishi.cn

echo "log" >> out.log
来源：http://acu.tarul.cn

[R41] 丢弃输出
来源：http://nuo.havefunace.top

cmd >/dev/null 2>&1
来源：http://jsv.ydjk.org.cn

[R42] 输入重定向
来源：http://jpq.haohaochexian.top

wc -l < a.txt
来源：http://omb.zdqjudy.top

[R43] 按名字查找文件
来源：http://wbt.aibaodan.cn

find . -name "*.log" -type f
来源：http://vtn.fehbvm.com

[R44] 按修改时间查找
来源：http://rqw.guannengcc.top

find . -mtime -7 -type f
来源：http://kwk.jianghu66.top

[R45] 批量删除
来源：http://pqb.daxiang520.top

find . -name "*.tmp" -delete
来源：http://vlx.hysaishi.cn

[R46] 递归替换文件内容
来源：http://xic.dashuyun.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://knj.chenlongwang.top

[R47] sed 单行替换
来源：http://hsu.ywan-chungtsiang.top

sed -i 's/foo/bar/g' a.txt
来源：http://esn.sweek.top

[R48] awk 取指定列
来源：http://isl.9152youxi.cn

awk '{print $1, $3}' a.txt
来源：http://gdz.shzxlz.cn

[R49] awk 带条件
来源：http://tlz.ybcxt.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ofe.hcnkem.com

[R50] awk 求和
来源：http://uju.zycfv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://azd.shangyingyoupin.top

[R51] 排序去重取前几
来源：http://etp.fktsv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://waw.shuidangran.top

[R52] 统计行数
来源：http://obr.zhixingplan.top

wc -l a.txt
来源：http://ldp.zhaomingkeji.xyz

[R53] 查看文件头与实时尾
来源：http://icd.daxiang520.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ycv.sjlbkw.cn

[R54] 比较两个文件
来源：http://euo.meibo888.top

diff a.txt b.txt
来源：http://rdj.guannengcc.top

[R55] 压缩与解压
来源：http://blv.yueranfly.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sgh.nwbrower.top

[R56] 远程拷贝
来源：http://ulp.sjlbkw.cn

scp file user@host:/path/
来源：http://cih.uphjek.com

[R57] 远程执行命令
来源：http://gww.yfazqb.com

ssh user@host 'uptime'
来源：http://nxq.ydzc1.top

[R58] 下载文件
来源：http://vuq.svipenyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nnc.shzxlz.cn

[R59] 发 POST JSON
来源：http://chb.jinqigfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uye.yj202588.top

[R60] 只看 HTTP 状态码
来源：http://qfa.cqqwz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kni.haohaochexian.top

[R61] 磁盘占用
来源：http://bdj.tanke756.top

df -h;  du -sh *
来源：http://fcu.aibaodan.cn

[R62] 找最占空间的文件
来源：http://bze.hammf.cn

du -ah . | sort -rh | head -10
来源：http://nny.dianchejie.cn

[R63] 内存与进程
来源：http://ghp.ywan-chungtsiang.top

free -h;  ps aux | grep nginx
来源：http://fnp.sweek.top

[R64] 结束进程
来源：http://gdn.nanxinkj.top

kill -9 $(pgrep -f app.py)
来源：http://nyp.fktsv.cn

[R65] 查看端口占用
来源：http://hzs.tarul.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gpf.hcnkem.com

[R66] 定时任务
来源：http://ird.tianlin.xyz

crontab -e;  crontab -l
来源：http://qbi.quarkkingdee.top

[R67] 生成随机十六进制串
来源：http://obp.cheryme.top

openssl rand -hex 16
来源：http://qgq.hnqzz.top

[R68] 计算文件校验值
来源：http://gvy.cashguo.top

sha256sum a.txt;  md5sum a.txt
来源：http://vla.yueranfly.top

[R69] 生成随机密码
来源：http://sns.hywenlv.cn

head -c 16 /dev/urandom | base64
来源：http://xhu.meibo888.top

[R70] 时间戳与互转
来源：http://ayv.sysykeji.top

date +%s;  date -d @1700000000
来源：http://jqp.tanke756.top

[R71] 日期格式化
来源：http://wyd.zycfv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yqt.wangshuangyany.cn

[R72] 等待端口就绪
来源：http://aad.gzhubu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://gtt.smart0.xyz

[R73] 分割大日志
来源：http://ete.tianlin.xyz

split -l 1000 big.log part_
来源：http://tph.hfpthk.cn

[R74] 批量重命名
来源：http://wio.sweek.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hzv.wangdashe.top

[R75] 导出环境变量
来源：http://akt.tian-w.cn

export PATH="$HOME/bin:$PATH"
来源：http://ljv.smart0.xyz

[R76] 使用临时文件
来源：http://ohf.iojbl.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eph.shangyingyoupin.top

[R77] 读取用户输入
来源：http://jfi.vehdjk.com

read -rp "请输入: " ans
来源：http://rfg.nanxuanxn.top

[R78] 交互式菜单
来源：http://zac.zhaomingkeji.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://gnz.xylfe.cn

[R79] 解析命令行选项
来源：http://lqw.shanyushiyangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bhf.xziqi.cn

[R80] 查看脚本执行耗时
来源：http://qbh.zdqjudy.top

time ./run.sh
来源：http://bcj.dianchejie.cn

================================================================================
来源：http://wen.shanyushiyangtech.top

S. C / C++ 专题
来源：http://hry.iojbl.cn

================================================================================
来源：http://fkw.chenjidiqi.icu

[S01] C：Hello World
来源：http://zcl.aibaodan.cn

#include <stdio.h>
来源：http://cft.cdnleiting.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jtk.dashuyun.cn

[S02] C：变量与格式化输出
来源：http://ack.fehbvm.com

int a = 10; printf("%d\n", a);
来源：http://ypo.yueranfly.top

[S03] C：读入整数
来源：http://ojj.yj20258.top

int x; scanf("%d", &x);
来源：http://zdq.sjlbkw.cn

[S04] C：字符串复制
来源：http://nip.gotoacloud.top

char dst[32]; strcpy(dst, "hi");
来源：http://azu.hywenlv.cn

[S05] C：字符串长度
来源：http://cra.tanke756.top

strlen(s)
来源：http://dmm.guannengcc.top

[S06] C：字符串比较
来源：http://jpw.jinqigufen.top

strcmp(a, b) == 0
来源：http://lrc.cheryme.top

[S07] C：数组遍历求和
来源：http://fre.shanyushiyangkeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wux.zhongyouzk.top

[S08] C：动态内存分配与释放
来源：http://btj.hcnkem.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vdn.hfpthk.cn

[S09] C：结构体定义与初始化
来源：http://kcd.sysykeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pqj.52xcode.cn

[S10] C：指针与解引用
来源：http://jxn.yueranfly.top

int *p = &a;  *p = 5;
来源：http://lxm.guannengcc.top

[S11] C：逐行读文件
来源：http://xcg.0kj1m.cn

FILE *f = fopen("a.txt", "r");
来源：http://pyb.sxryk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://stj.yj20258888.top

fclose(f);
来源：http://wvo.tanke756.top

[S12] C：写文件
来源：http://bkj.chenzaomai.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jow.yvedp.cn

[S13] C：宏定义
来源：http://dgq.iojbl.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lcl.smart0.xyz

[S14] C：枚举
来源：http://uqc.mhx1999.top

enum Color { RED, GREEN, BLUE };
来源：http://suz.sufxvd.cn

[S15] C：类型转换
来源：http://itr.zdbjq.cn

(double) a / b
来源：http://qgk.cheryme.top

[S16] C：位操作置位
来源：http://xio.yongpay.top

x |= (1 << 3);
来源：http://kyp.xylfe.cn

[S17] C：安全拼接字符串
来源：http://avu.sufxvd.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://boc.sysykeji.top

[S18] C：命令行参数
来源：http://xfr.nanxinkj.top

int main(int argc, char **argv)
来源：http://cyj.havefunace.top

[S19] C：快速排序
来源：http://edk.pengpengdd.cyou

qsort(a, n, sizeof(int), cmp);
来源：http://ebs.zhijiandao.cn

[S20] C：二分查找
来源：http://nje.52xcode.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://irq.hnxiangtu.top

[S21] C：字符类别判断
来源：http://eom.yj202588.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://adl.yj20258888.top

[S22] C：字符串转数字
来源：http://ehp.xuanzx.com

atoi("42");  strtod("3.14", NULL);
来源：http://xmo.zdbjq.cn

[S23] C：随机数
来源：http://myp.fktsv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yrq.jinqigufen.top

[S24] C：获取本地时间
来源：http://aeq.chenzaomai.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vse.ivvv.top

[S25] C：内存拷贝
来源：http://jgn.sysykeji.top

memcpy(dst, src, n);
来源：http://rlo.cucudq.cn

[S26] C：内存清零
来源：http://zbn.yongpay.top

memset(a, 0, sizeof a);
来源：http://rlm.jqgufenzy.top

[S27] C：定义常量
来源：http://oxw.jlsjyb.cn

const double PI = 3.14159;
来源：http://jre.pengpengdd.cyou

[S28] C：静态变量
来源：http://xzi.wangdashe.top


<!-- 参考信息 -->