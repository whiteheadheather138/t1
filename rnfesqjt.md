代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fll.quarkkingdee.top

[Q60] 取上一行 / 下一行
来源：http://fup.vehdjk.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wio.fktsv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jbj.shanyushiyangkeji.top

[Q61] 移动平均
来源：http://vrx.gogol.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nij.nanxinkj.top

[Q62] 分组占比
来源：http://aki.ywan-chungtsiang.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kbd.nanxuanxn.top

[Q63] 开启事务
来源：http://hdk.fanxiaobao.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://uvz.yvedp.cn

[Q64] 提交事务
来源：http://dcu.yanxiufei.cn

COMMIT;
来源：http://lvp.jianghu66.top

[Q65] 回滚事务
来源：http://nnc.hongshengwenyu.top

ROLLBACK;
来源：http://dpc.gaohongyu789.top

[Q66] 行锁查询
来源：http://ovb.nanxuanxn.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rxs.ivvv.top

[Q67] 设置隔离级别
来源：http://gdh.ivvv.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oqd.zhaomingkeji.xyz

[Q68] 保存点
来源：http://hbr.daria6918.cn

SAVEPOINT sp1;
来源：http://pmh.yvedp.cn

ROLLBACK TO sp1;
来源：http://ibh.feifeiyinyue.top

[Q69] 查看执行计划
来源：http://iuo.birdmap.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ead.wangdashe.top

[Q70] 更新统计信息
来源：http://yvf.meibo888.top

ANALYZE TABLE users;
来源：http://gcb.svipenyu.cn

[Q71] 查看建表语句
来源：http://puu.xuanzx.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zgg.uphjek.com

[Q72] 查看索引
来源：http://dlf.hammf.cn

SHOW INDEX FROM users;
来源：http://vll.xylfe.cn

[Q73] 查看表状态
来源：http://chf.jinqigfzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://kuk.feifeiyinyue.top

[Q74] 强制使用索引
来源：http://qgl.shuidangran.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lvx.tanke756.top

[Q75] 日期格式化
来源：http://osl.xinyue.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sxi.zdqjudy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lda.fanxiaobao.xyz

[Q76] 按天统计
来源：http://xdw.hnqzz.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tgk.zhaomingkeji.xyz

[Q77] 时间加减
来源：http://auw.svipenyu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sji.ivvv.top

[Q78] 当前时间
来源：http://trp.hcnkem.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ubd.jiagoushi.top

[Q79] 字符串拼接
来源：http://qem.yongpay.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://aad.jinqigfzy.top

[Q80] 字符串截取
来源：http://izh.jinqigufen.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wec.iojbl.cn

[Q81] 字符串替换
来源：http://fbf.ywan-chungtsiang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://api.316326.xyz

[Q82] 字符长度与字节长度
来源：http://bbu.hfpthk.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://awy.hnqzz.top

[Q83] 大小写转换
来源：http://jby.cdnleiting.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wqe.cashguo.top

[Q84] 去除首尾空格
来源：http://iib.yfazqb.com

SELECT TRIM(name) FROM users;
来源：http://twp.hfpthk.cn

[Q85] 数值取整
来源：http://nhu.daria6918.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qms.hnqzz.top

[Q86] 读取 JSON 字段
来源：http://ywq.sweek.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jrp.nanxinkj.top

[Q87] JSON 字段做条件
来源：http://puk.ehwqpu.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qbo.nanxinkj.top

[Q88] 行转列（条件聚合）
来源：http://fmq.snrcjt.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ppq.dianchejie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ppg.nanxinkj.top

[Q89] 判断表是否存在
来源：http://jaj.hammf.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://brv.hammf.cn

[Q90] 生成序号列
来源：http://bfe.jinqigufen.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dji.ydjk.org.cn

================================================================================
来源：http://npm.fanxiaobao.xyz

R. Bash 专题
来源：http://hsl.haohaochexian.top

================================================================================
来源：http://spe.daria6918.cn

[R01] shebang 与严格模式
来源：http://xii.bbcook.cn

#!/usr/bin/env bash
来源：http://ord.sxryk.cn

set -euo pipefail
来源：http://rsx.fanxiaobao.xyz

[R02] 变量赋值与使用
来源：http://pqz.tarul.cn

name="Tom"; echo "$name"
来源：http://fvz.redwolf501.top

[R03] 只读变量
来源：http://qvs.meibo888.top

readonly PI=3.14
来源：http://ije.gotoacloud.top

[R04] 位置参数
来源：http://eon.zhaomingkeji.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qte.chenjidiqi.icu

[R05] 参数默认值
来源：http://ojl.bbcook.cn

name="${1:-default}"
来源：http://cqx.fzhhl.top

[R06] 判断命令是否存在
来源：http://pfe.chenzaomai.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nkv.redwolf501.top

[R07] if 判断文件
来源：http://nyw.xylfe.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lct.tian-w.cn

[R08] 数值比较
来源：http://seo.hesvh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://onx.gogol.net.cn

[R09] 字符串比较
来源：http://nep.yuanzhike.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ton.jinqigfzy.top

[R10] 正则匹配
来源：http://uqm.zycfv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://afy.wangdashe.top

[R11] case 多分支
来源：http://yrp.zhengqikj.top

case "$1" in
来源：http://daq.sysykeji.top

start) echo "启动" ;;
来源：http://vmn.gotoacloud.top

stop)  echo "停止" ;;
来源：http://oos.svipenyu.cn

*)     echo "未知命令" ;;
来源：http://fjr.fengsongda.top

esac
来源：http://hmo.yuanzhike.top

[R12] for 遍历文件
来源：http://saq.gaohongyu789.top

for f in *.txt; do echo "$f"; done
来源：http://fdo.ywan-chungtsiang.top

[R13] for 计数循环
来源：http://qsy.kuanghao11.cn

for i in {1..10}; do echo "$i"; done
来源：http://mub.yuxming.cn

[R14] C 风格 for
来源：http://enr.zhengqikj.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://svz.daria6918.cn

[R15] while 逐行读文件
来源：http://wtp.fanxiaobao.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nse.zdbjq.cn

[R16] until 等待条件
来源：http://dzg.bjfxy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lpr.hywenlv.cn

[R17] 数组定义与取值
来源：http://zgo.daxiang520.top

arr=(a b c); echo "${arr[0]}"
来源：http://ecz.redwolf501.top

[R18] 遍历数组
来源：http://wpv.uphjek.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xbl.yvedp.cn

[R19] 数组长度
来源：http://jbj.zycfv.cn

echo "${#arr[@]}"
来源：http://fpf.jyoumei.cn

[R20] 关联数组（字典）
来源：http://jhs.hywenlv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://upg.uphjek.com

[R21] 字符串长度
来源：http://xxh.sufxvd.cn

echo "${#s}"
来源：http://wtt.fktsv.cn

[R22] 截取子串
来源：http://dqk.shanyushiyangtech.top

echo "${s:0:5}"
来源：http://bze.fanxiaobao.xyz

[R23] 字符串替换
来源：http://coj.jyoumei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qhh.daria6918.cn

[R24] 大小写转换
来源：http://tuv.yfazqb.com

echo "${s^^}"; echo "${s,,}"
来源：http://edk.vqdsnc.cn

[R25] 去后缀 / 去前缀
来源：http://laz.tarul.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qmb.haohaochexian.top

[R26] 命令替换
来源：http://eeq.ydjk.org.cn

now=$(date +%F); echo "$now"
来源：http://pds.yonumen.top

[R27] 算术展开
来源：http://psk.jqgufenzy.top

echo $((1 + 2 * 3))
来源：http://sjm.zdqjudy.top

[R28] 浮点运算
来源：http://tzi.gogol.net.cn

echo "scale=2; 10/3" | bc
来源：http://mwm.vqdsnc.cn

[R29] 定义函数
来源：http://aqf.cdnleiting.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kpu.tarul.cn

[R30] 函数返回状态码
来源：http://scu.tarul.cn

f() { return 0; }; f || echo "失败了"
来源：http://ymb.ehwqpu.com

[R31] 局部变量
来源：http://lme.316326.xyz

f() { local x=1; echo "$x"; }
来源：http://dzo.shzxlz.cn

[R32] 参数个数校验
来源：http://vha.hcnkem.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tkj.guannengcc.top

[R33] 捕获错误并提示行号
来源：http://ukn.jlsjyb.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oql.zhiwuduotai.top

[R34] 退出时清理
来源：http://puc.quarkkingdee.top

trap 'rm -f "$tmp"' EXIT
来源：http://yqj.haohaochexian.top

[R35] 后台执行并等待
来源：http://gxu.epnwcf.com

sleep 5 & pid=$!; wait "$pid"
来源：http://zpy.wangshuangyany.cn

[R36] 并发执行多个任务
来源：http://vyd.chenjidiqi.icu

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bkr.ppjwa.cn

[R37] 把输出赋给变量
来源：http://rpq.yanxiufei.cn

files=$(ls -1)
来源：http://mgd.jlsjyb.cn

[R38] 管道串联
来源：http://bfi.cqqwz.cn

cat a.txt | grep -i error | wc -l
来源：http://gop.sysykeji.top

[R39] 重定向标准输出与错误
来源：http://tkh.ywan-chungtsiang.top

cmd > out.log 2>&1
来源：http://pkw.gaohongyu789.top

[R40] 追加写日志
来源：http://mie.cheryme.top

echo "log" >> out.log
来源：http://oym.ppjwa.cn

[R41] 丢弃输出
来源：http://ntj.yangfankeji.com

cmd >/dev/null 2>&1
来源：http://ulg.birdmap.top

[R42] 输入重定向
来源：http://ytk.shangyingyoupin.top

wc -l < a.txt
来源：http://dtl.cucudq.cn

[R43] 按名字查找文件
来源：http://lbt.vehdjk.com

find . -name "*.log" -type f
来源：http://hmt.ybcxt.top

[R44] 按修改时间查找
来源：http://spa.svipenyu.cn

find . -mtime -7 -type f
来源：http://goz.jyoumei.cn

[R45] 批量删除
来源：http://fss.aizwys.cn

find . -name "*.tmp" -delete
来源：http://mnl.jinghuilouyu.cn

[R46] 递归替换文件内容
来源：http://rni.sjlbkw.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fqe.meibo888.top

[R47] sed 单行替换
来源：http://oxh.xinyue.icu

sed -i 's/foo/bar/g' a.txt
来源：http://gfj.hysaishi.cn

[R48] awk 取指定列
来源：http://yvl.cqqwz.cn

awk '{print $1, $3}' a.txt
来源：http://pmq.chenzaomai.com

[R49] awk 带条件
来源：http://lke.hammf.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rbi.wangshuangyany.cn

[R50] awk 求和
来源：http://dbd.shzxlz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://spv.chenjidiqi.icu

[R51] 排序去重取前几
来源：http://wnf.hywenlv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mjc.yueranfly.top

[R52] 统计行数
来源：http://dfj.yj20258888.top

wc -l a.txt
来源：http://oad.hammf.cn

[R53] 查看文件头与实时尾
来源：http://ttz.mhx1999.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xuv.chenjidiqi.icu

[R54] 比较两个文件
来源：http://mir.jinqigfzy.top

diff a.txt b.txt
来源：http://wah.hywenlv.cn

[R55] 压缩与解压
来源：http://nds.yanxiufei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dwv.9152youxi.cn

[R56] 远程拷贝
来源：http://qga.hammf.cn

scp file user@host:/path/
来源：http://ldw.havefunace.top

[R57] 远程执行命令
来源：http://xsc.c1oappe.top

ssh user@host 'uptime'
来源：http://rzh.gzhubu.top

[R58] 下载文件
来源：http://xne.gogol.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xwh.xylfe.cn

[R59] 发 POST JSON
来源：http://usf.ybcxt.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ppa.yj20258888.top

[R60] 只看 HTTP 状态码
来源：http://jpu.hnxiangtu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pnf.jiagoushi.top

[R61] 磁盘占用
来源：http://jiz.fengsongda.top

df -h;  du -sh *
来源：http://nts.aizwys.cn

[R62] 找最占空间的文件
来源：http://xpy.yvedp.cn

du -ah . | sort -rh | head -10
来源：http://igg.hnxiangtu.top

[R63] 内存与进程
来源：http://gzp.yangfankeji.com

free -h;  ps aux | grep nginx
来源：http://ywn.ydjk.org.cn

[R64] 结束进程
来源：http://pkt.zhijiandao.cn

kill -9 $(pgrep -f app.py)
来源：http://oab.c1oappe.top

[R65] 查看端口占用
来源：http://brv.mhx1999.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dzf.yanxiufei.cn

[R66] 定时任务
来源：http://bbn.ywan-chungtsiang.top

crontab -e;  crontab -l
来源：http://cwq.hfpthk.cn

[R67] 生成随机十六进制串
来源：http://mdy.zhongyouzk.top

openssl rand -hex 16
来源：http://rac.ctjpmb.com

[R68] 计算文件校验值
来源：http://lpq.vqdsnc.cn

sha256sum a.txt;  md5sum a.txt
来源：http://oqj.sweek.top

[R69] 生成随机密码
来源：http://hok.xuanzx.com

head -c 16 /dev/urandom | base64
来源：http://bey.zhoulong.xyz

[R70] 时间戳与互转
来源：http://pck.dianchejie.cn

date +%s;  date -d @1700000000
来源：http://opg.zhoulong.xyz

[R71] 日期格式化
来源：http://zby.shangyingyoupin.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://uto.cdnleiting.top

[R72] 等待端口就绪
来源：http://alh.zhongyouzk.top

until nc -z localhost 3306; do sleep 1; done
来源：http://chv.ctjpmb.com

[R73] 分割大日志
来源：http://ore.shanyushiyangkeji.top

split -l 1000 big.log part_
来源：http://yit.hcnkem.com

[R74] 批量重命名
来源：http://fad.yanxiufei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bvj.52xcode.cn

[R75] 导出环境变量
来源：http://qfz.bjfxy.top

export PATH="$HOME/bin:$PATH"
来源：http://jjd.tarul.cn

[R76] 使用临时文件
来源：http://ykm.xuanzx.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lpn.jyoumei.cn

[R77] 读取用户输入
来源：http://nzw.jqgufenzy.top

read -rp "请输入: " ans
来源：http://nsm.guannengcc.top

[R78] 交互式菜单
来源：http://ifa.jyoumei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gjq.feifeiyinyue.top

[R79] 解析命令行选项
来源：http://bmn.zdqjudy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zsj.zhengqikj.top

[R80] 查看脚本执行耗时
来源：http://rns.zhengqikj.top

time ./run.sh
来源：http://rai.jianghu66.top

================================================================================
来源：http://byu.vehdjk.com

S. C / C++ 专题
来源：http://jrc.nanxinkj.top

================================================================================
来源：http://whx.hywenlv.cn

[S01] C：Hello World
来源：http://vfd.xylfe.cn

#include <stdio.h>
来源：http://vcj.tanke756.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wmy.shzxlz.cn

[S02] C：变量与格式化输出
来源：http://knv.zdqjudy.top

int a = 10; printf("%d\n", a);
来源：http://wfe.sysykeji.top

[S03] C：读入整数
来源：http://epp.chenlongwang.top

int x; scanf("%d", &x);
来源：http://ulu.mhx1999.top

[S04] C：字符串复制
来源：http://msy.zdbjq.cn

char dst[32]; strcpy(dst, "hi");
来源：http://utw.yanxiufei.cn

[S05] C：字符串长度
来源：http://tmi.sjlbkw.cn

strlen(s)
来源：http://lku.ywan-chungtsiang.top

[S06] C：字符串比较
来源：http://edz.yanxiufei.cn

strcmp(a, b) == 0
来源：http://ebk.ppjwa.cn

[S07] C：数组遍历求和
来源：http://ukt.yuanzhike.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xas.zhoulong.xyz

[S08] C：动态内存分配与释放
来源：http://ggp.xuanzx.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kcp.nanxinkj.top

[S09] C：结构体定义与初始化
来源：http://mxt.ydzc1.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nod.aizwys.cn

[S10] C：指针与解引用
来源：http://mca.0kj1m.cn

int *p = &a;  *p = 5;
来源：http://osl.epnwcf.com

[S11] C：逐行读文件
来源：http://moi.ctjpmb.com

FILE *f = fopen("a.txt", "r");
来源：http://vtv.aizwys.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zaj.jinghuilouyu.cn

fclose(f);
来源：http://dhx.fzhhl.top

[S12] C：写文件
来源：http://pmx.birdmap.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vmf.yuanzhike.top

[S13] C：宏定义
来源：http://tyn.xylfe.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://snd.fehbvm.com

[S14] C：枚举
来源：http://xky.andypj.xyz

enum Color { RED, GREEN, BLUE };
来源：http://sck.ivvv.top

[S15] C：类型转换
来源：http://xsu.zhengqikj.top

(double) a / b
来源：http://xcg.xingfuxueyuan.xyz

[S16] C：位操作置位
来源：http://vdt.zhaomingkeji.xyz

x |= (1 << 3);
来源：http://yzz.havefunace.top

[S17] C：安全拼接字符串
来源：http://nxm.tanke756.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rpp.jiagoushi.top

[S18] C：命令行参数
来源：http://wrr.svipenyu.cn

int main(int argc, char **argv)
来源：http://gor.yongpay.top

[S19] C：快速排序
来源：http://xwo.yongpay.top

qsort(a, n, sizeof(int), cmp);
来源：http://fsk.cheryme.top

[S20] C：二分查找
来源：http://elq.wangdashe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gss.jianghu66.top

[S21] C：字符类别判断
来源：http://jte.kuanghao11.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mdb.wangdashe.top

[S22] C：字符串转数字
来源：http://zeo.shanyushiyangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://jfp.zhaomingkeji.xyz

[S23] C：随机数
来源：http://owt.sweek.top

srand(time(NULL));  int r = rand() % 100;
来源：http://utx.ctjpmb.com

[S24] C：获取本地时间
来源：http://byz.sufxvd.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://btk.guannengcc.top

[S25] C：内存拷贝
来源：http://jnq.sysykeji.top

memcpy(dst, src, n);
来源：http://apg.andypj.xyz

[S26] C：内存清零
来源：http://bkp.hesvh.cn

memset(a, 0, sizeof a);
来源：http://rzx.haohaochexian.top

[S27] C：定义常量
来源：http://kut.zycfv.cn

const double PI = 3.14159;
来源：http://yxn.52xcode.cn

[S28] C：静态变量
来源：http://zee.hysaishi.cn

static int counter = 0;
来源：http://ijc.tian-w.cn

[S29] C：变参函数
来源：http://wma.hnqzz.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ydg.jyoumei.cn

[S30] C：头文件保护
来源：http://kva.smart0.xyz


<!-- 参考信息 -->