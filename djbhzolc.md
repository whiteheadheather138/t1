代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wqw.shuidangran.top

[Q60] 取上一行 / 下一行
来源：http://qdq.52xcode.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ack.vehdjk.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jyp.aibaodan.cn

[Q61] 移动平均
来源：http://wdo.smart0.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qzu.hongshengwenyu.top

[Q62] 分组占比
来源：http://mew.sufxvd.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xxh.fehbvm.com

[Q63] 开启事务
来源：http://fli.c1oappe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fnj.cheryme.top

[Q64] 提交事务
来源：http://mqd.zhijiandao.cn

COMMIT;
来源：http://uej.yuxming.cn

[Q65] 回滚事务
来源：http://mwa.pycfn.com

ROLLBACK;
来源：http://seg.52xcode.cn

[Q66] 行锁查询
来源：http://kjn.hywenlv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xow.shzxlz.cn

[Q67] 设置隔离级别
来源：http://yve.pycfn.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://erl.yj20258888.top

[Q68] 保存点
来源：http://aqn.daria6918.cn

SAVEPOINT sp1;
来源：http://glv.zhiwuduotai.top

ROLLBACK TO sp1;
来源：http://otf.fktsv.cn

[Q69] 查看执行计划
来源：http://zfp.xziqi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ofy.hcnkem.com

[Q70] 更新统计信息
来源：http://toe.guowangkeji.top

ANALYZE TABLE users;
来源：http://wsw.nanxuanxn.top

[Q71] 查看建表语句
来源：http://waf.xingfuxueyuan.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hci.52xcode.cn

[Q72] 查看索引
来源：http://eqv.yuanzhike.top

SHOW INDEX FROM users;
来源：http://kck.cashguo.top

[Q73] 查看表状态
来源：http://kmv.guowangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://koq.hnqzz.top

[Q74] 强制使用索引
来源：http://qtg.shuidangran.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gay.kuanghao11.cn

[Q75] 日期格式化
来源：http://ipt.pengpengdd.cyou

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pma.chenlongwang.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kcb.sufxvd.cn

[Q76] 按天统计
来源：http://qty.iojbl.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lsz.gotoacloud.top

[Q77] 时间加减
来源：http://xdm.gotoacloud.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zgy.snrcjt.cn

[Q78] 当前时间
来源：http://oil.jqgufenzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gjl.smart0.xyz

[Q79] 字符串拼接
来源：http://sgu.hfpthk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yfp.gogol.net.cn

[Q80] 字符串截取
来源：http://cwq.yongpay.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lek.hfpthk.cn

[Q81] 字符串替换
来源：http://gmc.sysykeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://goy.jianghu66.top

[Q82] 字符长度与字节长度
来源：http://qvy.jianghu66.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nbl.birdmap.top

[Q83] 大小写转换
来源：http://kgx.jyoumei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lis.c1oappe.top

[Q84] 去除首尾空格
来源：http://aba.fzhhl.top

SELECT TRIM(name) FROM users;
来源：http://hym.aibaodan.cn

[Q85] 数值取整
来源：http://rxw.hfpthk.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iao.yonumen.top

[Q86] 读取 JSON 字段
来源：http://epi.cqqwz.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xfo.shuidangran.top

[Q87] JSON 字段做条件
来源：http://jqf.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://raa.ywan-chungtsiang.top

[Q88] 行转列（条件聚合）
来源：http://hjv.zdbjq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wpk.hywenlv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hle.ywan-chungtsiang.top

[Q89] 判断表是否存在
来源：http://fnz.jinyuanbaomall.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jwo.wangdashe.top

[Q90] 生成序号列
来源：http://eta.havefunace.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gxc.sxryk.cn

================================================================================
来源：http://llq.zhaomingkeji.xyz

R. Bash 专题
来源：http://rro.fktsv.cn

================================================================================
来源：http://jqy.zdqjudy.top

[R01] shebang 与严格模式
来源：http://ruj.yj20258888.top

#!/usr/bin/env bash
来源：http://amk.jinyuanbaomall.cn

set -euo pipefail
来源：http://abb.meibo888.top

[R02] 变量赋值与使用
来源：http://lcl.chenlongwang.top

name="Tom"; echo "$name"
来源：http://rrg.guowangkeji.top

[R03] 只读变量
来源：http://gfw.yuanzhike.top

readonly PI=3.14
来源：http://isz.ehwqpu.com

[R04] 位置参数
来源：http://wag.52xcode.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://isj.bbcook.cn

[R05] 参数默认值
来源：http://jdj.aizwys.cn

name="${1:-default}"
来源：http://yrb.guannengcc.top

[R06] 判断命令是否存在
来源：http://sej.zdbjq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zaa.sysykeji.top

[R07] if 判断文件
来源：http://bxp.gogol.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qur.ehwqpu.com

[R08] 数值比较
来源：http://vws.zdbjq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ixw.sysykeji.top

[R09] 字符串比较
来源：http://uxw.dianchejie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zke.xuanzx.com

[R10] 正则匹配
来源：http://cfs.shzxlz.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://met.cucudq.cn

[R11] case 多分支
来源：http://nvy.jianghu66.top

case "$1" in
来源：http://mrn.316326.xyz

start) echo "启动" ;;
来源：http://zik.jinyuanbaomall.cn

stop)  echo "停止" ;;
来源：http://pgz.ehwqpu.com

*)     echo "未知命令" ;;
来源：http://dae.9152youxi.cn

esac
来源：http://ebv.jianghu66.top

[R12] for 遍历文件
来源：http://woq.jqgufenzy.top

for f in *.txt; do echo "$f"; done
来源：http://gwu.xuetiantiany.cn

[R13] for 计数循环
来源：http://zpw.zhiwuduotai.top

for i in {1..10}; do echo "$i"; done
来源：http://mki.zhiwuduotai.top

[R14] C 风格 for
来源：http://bgr.jinghuilouyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rlt.jinyuanbaomall.cn

[R15] while 逐行读文件
来源：http://nsd.zdqjudy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://spj.aibaodan.cn

[R16] until 等待条件
来源：http://udp.xingfuxueyuan.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jmx.xinyue.icu

[R17] 数组定义与取值
来源：http://jrh.guannengcc.top

arr=(a b c); echo "${arr[0]}"
来源：http://lkd.hongshengwenyu.top

[R18] 遍历数组
来源：http://cnz.hesvh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hsq.yueranfly.top

[R19] 数组长度
来源：http://dzc.yvedp.cn

echo "${#arr[@]}"
来源：http://kkn.hnqzz.top

[R20] 关联数组（字典）
来源：http://mer.316326.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aol.meibo888.top

[R21] 字符串长度
来源：http://phv.yj20258.top

echo "${#s}"
来源：http://ken.cdnleiting.top

[R22] 截取子串
来源：http://mrn.haohaochexian.top

echo "${s:0:5}"
来源：http://wkn.9152youxi.cn

[R23] 字符串替换
来源：http://ejq.feifeiyinyue.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mbx.sxryk.cn

[R24] 大小写转换
来源：http://eza.cdnleiting.top

echo "${s^^}"; echo "${s,,}"
来源：http://qll.daxiang520.top

[R25] 去后缀 / 去前缀
来源：http://ntv.wangdashe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://gxe.jianghu66.top

[R26] 命令替换
来源：http://hfp.guowangkeji.top

now=$(date +%F); echo "$now"
来源：http://ilk.jlsjyb.cn

[R27] 算术展开
来源：http://nxg.316326.xyz

echo $((1 + 2 * 3))
来源：http://iyg.cucudq.cn

[R28] 浮点运算
来源：http://xvm.nanxinkj.top

echo "scale=2; 10/3" | bc
来源：http://dcq.hysaishi.cn

[R29] 定义函数
来源：http://eas.tanke756.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tse.fengsongda.top

[R30] 函数返回状态码
来源：http://hvx.nwbrower.top

f() { return 0; }; f || echo "失败了"
来源：http://wfo.fzhhl.top

[R31] 局部变量
来源：http://rni.gaohongyu789.top

f() { local x=1; echo "$x"; }
来源：http://nwc.jyoumei.cn

[R32] 参数个数校验
来源：http://wmf.zhongyouzk.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ies.havefunace.top

[R33] 捕获错误并提示行号
来源：http://wjd.hammf.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tis.jqgfzy.top

[R34] 退出时清理
来源：http://zxf.gotoacloud.top

trap 'rm -f "$tmp"' EXIT
来源：http://mzj.snrcjt.cn

[R35] 后台执行并等待
来源：http://onn.haohaochexian.top

sleep 5 & pid=$!; wait "$pid"
来源：http://arz.ybcxt.top

[R36] 并发执行多个任务
来源：http://ufe.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://diz.dashuyun.cn

[R37] 把输出赋给变量
来源：http://wli.yueranfly.top

files=$(ls -1)
来源：http://evx.fanxiaobao.xyz

[R38] 管道串联
来源：http://pnz.hesvh.cn

cat a.txt | grep -i error | wc -l
来源：http://ukd.sxryk.cn

[R39] 重定向标准输出与错误
来源：http://shi.shanyushiyangtech.top

cmd > out.log 2>&1
来源：http://yru.chenjidiqi.icu

[R40] 追加写日志
来源：http://uen.yongpay.top

echo "log" >> out.log
来源：http://wms.hywenlv.cn

[R41] 丢弃输出
来源：http://sgm.wangdashe.top

cmd >/dev/null 2>&1
来源：http://ier.shzxlz.cn

[R42] 输入重定向
来源：http://zxr.ivvv.top

wc -l < a.txt
来源：http://snm.jianghu66.top

[R43] 按名字查找文件
来源：http://oai.ehwqpu.com

find . -name "*.log" -type f
来源：http://kag.yuanzhike.top

[R44] 按修改时间查找
来源：http://iow.kuanghao11.cn

find . -mtime -7 -type f
来源：http://sgr.sxryk.cn

[R45] 批量删除
来源：http://zvy.uphjek.com

find . -name "*.tmp" -delete
来源：http://ubn.yj202588.top

[R46] 递归替换文件内容
来源：http://zig.zycfv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jrn.ydzc1.top

[R47] sed 单行替换
来源：http://otb.sjlbkw.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pud.jinqigufen.top

[R48] awk 取指定列
来源：http://xdj.svipenyu.cn

awk '{print $1, $3}' a.txt
来源：http://rvp.hongshengwenyu.top

[R49] awk 带条件
来源：http://kea.tanke756.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vqn.birdmap.top

[R50] awk 求和
来源：http://asq.yangfankeji.com

awk '{s += $2} END {print s}' a.txt
来源：http://uke.pycfn.com

[R51] 排序去重取前几
来源：http://vuf.fktsv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ajg.sysykeji.top

[R52] 统计行数
来源：http://ynk.jyoumei.cn

wc -l a.txt
来源：http://emo.birdmap.top

[R53] 查看文件头与实时尾
来源：http://nwv.hesvh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jfh.fzhhl.top

[R54] 比较两个文件
来源：http://pvp.fengsongda.top

diff a.txt b.txt
来源：http://cro.yuanzhike.top

[R55] 压缩与解压
来源：http://jck.hysaishi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ngp.meibo888.top

[R56] 远程拷贝
来源：http://sph.cucudq.cn

scp file user@host:/path/
来源：http://yxe.hywenlv.cn

[R57] 远程执行命令
来源：http://gqc.shzxlz.cn

ssh user@host 'uptime'
来源：http://kwj.yuanzhike.top

[R58] 下载文件
来源：http://omi.shanyushiyangkeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ytx.cqqwz.cn

[R59] 发 POST JSON
来源：http://jzr.dashuyun.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gns.zhaomingkeji.xyz

[R60] 只看 HTTP 状态码
来源：http://lvp.ppjwa.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zlw.shanyushiyangtech.top

[R61] 磁盘占用
来源：http://wby.tarul.cn

df -h;  du -sh *
来源：http://xbd.xingfuxueyuan.xyz

[R62] 找最占空间的文件
来源：http://qrx.ydzc1.top

du -ah . | sort -rh | head -10
来源：http://gws.gogol.net.cn

[R63] 内存与进程
来源：http://nag.aizwys.cn

free -h;  ps aux | grep nginx
来源：http://fzc.gotoacloud.top

[R64] 结束进程
来源：http://csd.yfazqb.com

kill -9 $(pgrep -f app.py)
来源：http://rlh.fehbvm.com

[R65] 查看端口占用
来源：http://ykj.hnxiangtu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gte.wangshuangyany.cn

[R66] 定时任务
来源：http://xzy.shzxlz.cn

crontab -e;  crontab -l
来源：http://qzq.cashguo.top

[R67] 生成随机十六进制串
来源：http://yhv.nanxuanxn.top

openssl rand -hex 16
来源：http://gxx.hesvh.cn

[R68] 计算文件校验值
来源：http://yfr.zdbjq.cn

sha256sum a.txt;  md5sum a.txt
来源：http://usn.sjlbkw.cn

[R69] 生成随机密码
来源：http://bgs.jlsjyb.cn

head -c 16 /dev/urandom | base64
来源：http://zlb.zhaomingkeji.xyz

[R70] 时间戳与互转
来源：http://jgz.tianlin.xyz

date +%s;  date -d @1700000000
来源：http://rjg.ctjpmb.com

[R71] 日期格式化
来源：http://bit.jinghuilouyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nsv.yangfankeji.com

[R72] 等待端口就绪
来源：http://xix.vehdjk.com

until nc -z localhost 3306; do sleep 1; done
来源：http://zrz.yj202588.top

[R73] 分割大日志
来源：http://fda.nanxuanxn.top

split -l 1000 big.log part_
来源：http://owi.chenzaomai.com

[R74] 批量重命名
来源：http://ymc.hysaishi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vkj.ivvv.top

[R75] 导出环境变量
来源：http://gmj.haohaochexian.top

export PATH="$HOME/bin:$PATH"
来源：http://wwm.smart0.xyz

[R76] 使用临时文件
来源：http://dtl.sufxvd.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ryn.cdnleiting.top

[R77] 读取用户输入
来源：http://uad.ehwqpu.com

read -rp "请输入: " ans
来源：http://ilu.hnxiangtu.top

[R78] 交互式菜单
来源：http://zto.bjfxy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mwv.gaohongyu789.top

[R79] 解析命令行选项
来源：http://isr.mhx1999.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dff.fengsongda.top

[R80] 查看脚本执行耗时
来源：http://wmi.hesvh.cn

time ./run.sh
来源：http://oxn.dashuyun.cn

================================================================================
来源：http://frc.yonumen.top

S. C / C++ 专题
来源：http://guu.svipenyu.cn

================================================================================
来源：http://bym.zhiwuduotai.top

[S01] C：Hello World
来源：http://psn.ctjpmb.com

#include <stdio.h>
来源：http://xhx.shuidangran.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://quu.zhoulong.xyz

[S02] C：变量与格式化输出
来源：http://eap.zhengqikj.top

int a = 10; printf("%d\n", a);
来源：http://jtv.meibo888.top

[S03] C：读入整数
来源：http://gvp.zhoulong.xyz

int x; scanf("%d", &x);
来源：http://ryv.redwolf501.top

[S04] C：字符串复制
来源：http://tmu.sweek.top

char dst[32]; strcpy(dst, "hi");
来源：http://njd.hfpthk.cn

[S05] C：字符串长度
来源：http://gue.tarul.cn

strlen(s)
来源：http://ltz.uphjek.com

[S06] C：字符串比较
来源：http://xmx.tianlin.xyz

strcmp(a, b) == 0
来源：http://yqs.cqqwz.cn

[S07] C：数组遍历求和
来源：http://nyr.ybcxt.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ocg.meibo888.top

[S08] C：动态内存分配与释放
来源：http://mhb.yueranfly.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bxe.bjfxy.top

[S09] C：结构体定义与初始化
来源：http://mtf.xziqi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kgc.bbcook.cn

[S10] C：指针与解引用
来源：http://cam.shangyingyoupin.top

int *p = &a;  *p = 5;
来源：http://ylx.feifeiyinyue.top

[S11] C：逐行读文件
来源：http://nwy.gotoacloud.top

FILE *f = fopen("a.txt", "r");
来源：http://evj.guowangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nkr.fktsv.cn

fclose(f);
来源：http://sjm.svipenyu.cn

[S12] C：写文件
来源：http://sov.smart0.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yww.aibaodan.cn

[S13] C：宏定义
来源：http://kzy.shangyingyoupin.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://die.gotoacloud.top

[S14] C：枚举
来源：http://mje.smart0.xyz

enum Color { RED, GREEN, BLUE };
来源：http://nlf.zdqjudy.top

[S15] C：类型转换
来源：http://krj.nwbrower.top

(double) a / b
来源：http://ksu.wangshuangyany.cn

[S16] C：位操作置位
来源：http://afu.zhongyouzk.top

x |= (1 << 3);
来源：http://tnk.ivvv.top

[S17] C：安全拼接字符串
来源：http://qpx.zhijiandao.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qys.chenlongwang.top

[S18] C：命令行参数
来源：http://txh.yj20258888.top

int main(int argc, char **argv)
来源：http://zek.fehbvm.com

[S19] C：快速排序
来源：http://cug.epnwcf.com

qsort(a, n, sizeof(int), cmp);
来源：http://mbw.aizwys.cn

[S20] C：二分查找
来源：http://usy.iojbl.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://aow.andypj.xyz

[S21] C：字符类别判断
来源：http://amd.smart0.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vzh.tian-w.cn

[S22] C：字符串转数字
来源：http://bqm.cashguo.top

atoi("42");  strtod("3.14", NULL);
来源：http://sce.tianlin.xyz

[S23] C：随机数
来源：http://dbv.hywenlv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rkh.tianlin.xyz

[S24] C：获取本地时间
来源：http://ruo.ctjpmb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://svk.cqqwz.cn

[S25] C：内存拷贝
来源：http://qfu.jinyuanbaomall.cn

memcpy(dst, src, n);
来源：http://sfr.wangshuangyany.cn

[S26] C：内存清零
来源：http://geq.meibo888.top

memset(a, 0, sizeof a);
来源：http://fag.pycfn.com

[S27] C：定义常量
来源：http://ila.shanyushiyangkeji.top

const double PI = 3.14159;
来源：http://hzz.yanxiufei.cn

[S28] C：静态变量
来源：http://ybb.9152youxi.cn

static int counter = 0;
来源：http://ixw.ybcxt.top

[S29] C：变参函数
来源：http://dzb.fktsv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vpq.ydjk.org.cn

[S30] C：头文件保护
来源：http://sgj.xuetiantiany.cn


<!-- 参考信息 -->