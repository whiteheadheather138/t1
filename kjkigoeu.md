代发 wailian999

[Q63] 开启事务
来源：http://lce.tarul.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://non.kuanghao11.cn

[Q64] 提交事务
来源：http://scu.gotoacloud.top

COMMIT;
来源：http://aia.cheryme.top

[Q65] 回滚事务
来源：http://nyl.gzhubu.top

ROLLBACK;
来源：http://dud.bbcook.cn

[Q66] 行锁查询
来源：http://kvs.dashuyun.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dtk.dianchejie.cn

[Q67] 设置隔离级别
来源：http://wkw.jqgfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://awk.ydzc1.top

[Q68] 保存点
来源：http://nrd.meibo888.top

SAVEPOINT sp1;
来源：http://yah.zycfv.cn

ROLLBACK TO sp1;
来源：http://bka.nanxuanxn.top

[Q69] 查看执行计划
来源：http://pgb.vehdjk.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pns.fktsv.cn

[Q70] 更新统计信息
来源：http://apf.guowangkeji.top

ANALYZE TABLE users;
来源：http://wpu.yuxming.cn

[Q71] 查看建表语句
来源：http://mkv.smart0.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nlq.aizwys.cn

[Q72] 查看索引
来源：http://ahk.cheryme.top

SHOW INDEX FROM users;
来源：http://aso.chenlongwang.top

[Q73] 查看表状态
来源：http://lpk.zhongyouzk.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mbh.nwbrower.top

[Q74] 强制使用索引
来源：http://boo.nanxuanxn.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bbn.pengpengdd.cyou

[Q75] 日期格式化
来源：http://tyv.yvedp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xmg.jlsjyb.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yoh.jyoumei.cn

[Q76] 按天统计
来源：http://acr.xingfuxueyuan.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xtc.yj20258888.top

[Q77] 时间加减
来源：http://zns.c1oappe.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mhu.yanxiufei.cn

[Q78] 当前时间
来源：http://die.cqqwz.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zcp.shanyushiyangkeji.top

[Q79] 字符串拼接
来源：http://esf.yanxiufei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mqd.ywan-chungtsiang.top

[Q80] 字符串截取
来源：http://umn.ctjpmb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hsc.fengsongda.top

[Q81] 字符串替换
来源：http://pif.yuanzhike.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://znm.jlsjyb.cn

[Q82] 字符长度与字节长度
来源：http://fig.gogol.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kid.hysaishi.cn

[Q83] 大小写转换
来源：http://vyf.tarul.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fzi.hysaishi.cn

[Q84] 去除首尾空格
来源：http://xhl.316326.xyz

SELECT TRIM(name) FROM users;
来源：http://uor.ehwqpu.com

[Q85] 数值取整
来源：http://srb.bjfxy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wgq.fktsv.cn

[Q86] 读取 JSON 字段
来源：http://fbg.yueranfly.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kvc.0kj1m.cn

[Q87] JSON 字段做条件
来源：http://vck.hnxiangtu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://azs.nwbrower.top

[Q88] 行转列（条件聚合）
来源：http://tph.jinyuanbaomall.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yhc.quarkkingdee.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gek.nwbrower.top

[Q89] 判断表是否存在
来源：http://mds.zhengqikj.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://abc.svipenyu.cn

[Q90] 生成序号列
来源：http://szy.chenjidiqi.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lhl.yj202588.top

================================================================================
来源：http://zid.guannengcc.top

R. Bash 专题
来源：http://cdv.zdqjudy.top

================================================================================
来源：http://tmn.zhijiandao.cn

[R01] shebang 与严格模式
来源：http://kja.xingfuxueyuan.xyz

#!/usr/bin/env bash
来源：http://txs.aibaodan.cn

set -euo pipefail
来源：http://pdx.fengsongda.top

[R02] 变量赋值与使用
来源：http://qvu.yfazqb.com

name="Tom"; echo "$name"
来源：http://trc.nanxinkj.top

[R03] 只读变量
来源：http://bgl.cqqwz.cn

readonly PI=3.14
来源：http://vdi.ybcxt.top

[R04] 位置参数
来源：http://ugi.xuanzx.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://smr.yj20258888.top

[R05] 参数默认值
来源：http://cie.haohaochexian.top

name="${1:-default}"
来源：http://fwx.wangshuangyany.cn

[R06] 判断命令是否存在
来源：http://hwa.yuanzhike.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vmj.c1oappe.top

[R07] if 判断文件
来源：http://wij.ydzc1.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jyj.fzhhl.top

[R08] 数值比较
来源：http://spf.fanxiaobao.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://yrw.jlsjyb.cn

[R09] 字符串比较
来源：http://siu.yanxiufei.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gcu.aizwys.cn

[R10] 正则匹配
来源：http://hnp.zdqjudy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lxm.sysykeji.top

[R11] case 多分支
来源：http://omk.zhijiandao.cn

case "$1" in
来源：http://axh.zhiwuduotai.top

start) echo "启动" ;;
来源：http://ykg.redwolf501.top

stop)  echo "停止" ;;
来源：http://qdx.316326.xyz

*)     echo "未知命令" ;;
来源：http://nct.zdbjq.cn

esac
来源：http://tej.shanyushiyangkeji.top

[R12] for 遍历文件
来源：http://tjz.316326.xyz

for f in *.txt; do echo "$f"; done
来源：http://vli.52xcode.cn

[R13] for 计数循环
来源：http://sxc.fktsv.cn

for i in {1..10}; do echo "$i"; done
来源：http://nbk.sxryk.cn

[R14] C 风格 for
来源：http://iua.feifeiyinyue.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ktz.gaohongyu789.top

[R15] while 逐行读文件
来源：http://asa.daxiang520.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://shi.jyoumei.cn

[R16] until 等待条件
来源：http://dut.yangfankeji.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fan.jinghuilouyu.cn

[R17] 数组定义与取值
来源：http://efe.gaohongyu789.top

arr=(a b c); echo "${arr[0]}"
来源：http://ldj.xinyue.icu

[R18] 遍历数组
来源：http://ron.dashuyun.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://las.nanxuanxn.top

[R19] 数组长度
来源：http://fet.hesvh.cn

echo "${#arr[@]}"
来源：http://csi.quarkkingdee.top

[R20] 关联数组（字典）
来源：http://wdk.yuanzhike.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nzt.xuanzx.com

[R21] 字符串长度
来源：http://cem.hnxiangtu.top

echo "${#s}"
来源：http://hgk.uphjek.com

[R22] 截取子串
来源：http://eud.0kj1m.cn

echo "${s:0:5}"
来源：http://dpd.jinghuilouyu.cn

[R23] 字符串替换
来源：http://rgv.sxryk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lnj.cqqwz.cn

[R24] 大小写转换
来源：http://lex.snrcjt.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rwi.sufxvd.cn

[R25] 去后缀 / 去前缀
来源：http://kfy.hesvh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cos.fengsongda.top

[R26] 命令替换
来源：http://qun.yongpay.top

now=$(date +%F); echo "$now"
来源：http://fws.ywan-chungtsiang.top

[R27] 算术展开
来源：http://zqm.gzhubu.top

echo $((1 + 2 * 3))
来源：http://udr.xylfe.cn

[R28] 浮点运算
来源：http://lmy.aizwys.cn

echo "scale=2; 10/3" | bc
来源：http://abv.shzxlz.cn

[R29] 定义函数
来源：http://upy.c1oappe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://quh.birdmap.top

[R30] 函数返回状态码
来源：http://iyq.hcnkem.com

f() { return 0; }; f || echo "失败了"
来源：http://wqg.xylfe.cn

[R31] 局部变量
来源：http://abp.316326.xyz

f() { local x=1; echo "$x"; }
来源：http://gkw.yongpay.top

[R32] 参数个数校验
来源：http://jkx.cdnleiting.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fls.zycfv.cn

[R33] 捕获错误并提示行号
来源：http://ulh.shuidangran.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://amr.shanyushiyangkeji.top

[R34] 退出时清理
来源：http://vst.zdqjudy.top

trap 'rm -f "$tmp"' EXIT
来源：http://ylu.jqgufenzy.top

[R35] 后台执行并等待
来源：http://lxg.shanyushiyangtech.top

sleep 5 & pid=$!; wait "$pid"
来源：http://tgr.hfpthk.cn

[R36] 并发执行多个任务
来源：http://mzq.aibaodan.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qse.yongpay.top

[R37] 把输出赋给变量
来源：http://heo.wangdashe.top

files=$(ls -1)
来源：http://ggs.zhongyouzk.top

[R38] 管道串联
来源：http://ybt.xylfe.cn

cat a.txt | grep -i error | wc -l
来源：http://czh.zhijiandao.cn

[R39] 重定向标准输出与错误
来源：http://gsc.chenlongwang.top

cmd > out.log 2>&1
来源：http://rla.yuxming.cn

[R40] 追加写日志
来源：http://vfy.tian-w.cn

echo "log" >> out.log
来源：http://bvw.sxryk.cn

[R41] 丢弃输出
来源：http://owi.yanxiufei.cn

cmd >/dev/null 2>&1
来源：http://esn.gzhubu.top

[R42] 输入重定向
来源：http://fri.ivvv.top

wc -l < a.txt
来源：http://tia.zycfv.cn

[R43] 按名字查找文件
来源：http://zvu.gotoacloud.top

find . -name "*.log" -type f
来源：http://mvc.gogol.net.cn

[R44] 按修改时间查找
来源：http://ngo.yuanzhike.top

find . -mtime -7 -type f
来源：http://zxs.snrcjt.cn

[R45] 批量删除
来源：http://hsk.dianchejie.cn

find . -name "*.tmp" -delete
来源：http://wnk.chenjidiqi.icu

[R46] 递归替换文件内容
来源：http://hne.yangfankeji.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mlm.mhx1999.top

[R47] sed 单行替换
来源：http://kod.zdbjq.cn

sed -i 's/foo/bar/g' a.txt
来源：http://owz.redwolf501.top

[R48] awk 取指定列
来源：http://qla.52xcode.cn

awk '{print $1, $3}' a.txt
来源：http://sba.xuanzx.com

[R49] awk 带条件
来源：http://ajw.pycfn.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zps.shuidangran.top

[R50] awk 求和
来源：http://wbc.xinyue.icu

awk '{s += $2} END {print s}' a.txt
来源：http://qiq.yongpay.top

[R51] 排序去重取前几
来源：http://ixm.yuanzhike.top

sort a.txt | uniq -c | sort -rn | head
来源：http://emw.shanyushiyangtech.top

[R52] 统计行数
来源：http://cgh.svipenyu.cn

wc -l a.txt
来源：http://hhs.chenlongwang.top

[R53] 查看文件头与实时尾
来源：http://omj.bbcook.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mce.daria6918.cn

[R54] 比较两个文件
来源：http://bpi.snrcjt.cn

diff a.txt b.txt
来源：http://txl.wangshuangyany.cn

[R55] 压缩与解压
来源：http://shq.hnqzz.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hye.haohaochexian.top

[R56] 远程拷贝
来源：http://bpw.hnqzz.top

scp file user@host:/path/
来源：http://lbi.jqgfzy.top

[R57] 远程执行命令
来源：http://vin.uphjek.com

ssh user@host 'uptime'
来源：http://pgr.yvedp.cn

[R58] 下载文件
来源：http://ljp.feifeiyinyue.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sth.hnxiangtu.top

[R59] 发 POST JSON
来源：http://hcf.0kj1m.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gli.chenlongwang.top

[R60] 只看 HTTP 状态码
来源：http://rws.vehdjk.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sgj.jyoumei.cn

[R61] 磁盘占用
来源：http://vet.chenzaomai.com

df -h;  du -sh *
来源：http://rjd.snrcjt.cn

[R62] 找最占空间的文件
来源：http://lrt.guowangkeji.top

du -ah . | sort -rh | head -10
来源：http://sli.ywan-chungtsiang.top

[R63] 内存与进程
来源：http://kro.nwbrower.top

free -h;  ps aux | grep nginx
来源：http://gaj.jinqigufen.top

[R64] 结束进程
来源：http://psm.vehdjk.com

kill -9 $(pgrep -f app.py)
来源：http://ewz.zhiwuduotai.top

[R65] 查看端口占用
来源：http://jfx.ppjwa.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kez.sxryk.cn

[R66] 定时任务
来源：http://ids.nanxuanxn.top

crontab -e;  crontab -l
来源：http://rku.jinghuilouyu.cn

[R67] 生成随机十六进制串
来源：http://edp.dashuyun.cn

openssl rand -hex 16
来源：http://obm.sjlbkw.cn

[R68] 计算文件校验值
来源：http://oxa.dianchejie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fgj.dianchejie.cn

[R69] 生成随机密码
来源：http://xql.dashuyun.cn

head -c 16 /dev/urandom | base64
来源：http://szt.hnxiangtu.top

[R70] 时间戳与互转
来源：http://kdw.yueranfly.top

date +%s;  date -d @1700000000
来源：http://oqc.zhijiandao.cn

[R71] 日期格式化
来源：http://mbv.ydzc1.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://eom.316326.xyz

[R72] 等待端口就绪
来源：http://okr.yuxming.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ejm.pycfn.com

[R73] 分割大日志
来源：http://xdx.sweek.top

split -l 1000 big.log part_
来源：http://kno.gotoacloud.top

[R74] 批量重命名
来源：http://ecm.epnwcf.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fjd.gotoacloud.top

[R75] 导出环境变量
来源：http://hru.jinqigufen.top

export PATH="$HOME/bin:$PATH"
来源：http://kup.uphjek.com

[R76] 使用临时文件
来源：http://bfl.ydjk.org.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qzk.fehbvm.com

[R77] 读取用户输入
来源：http://ibh.hesvh.cn

read -rp "请输入: " ans
来源：http://zxn.fktsv.cn

[R78] 交互式菜单
来源：http://dos.fktsv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vch.bbcook.cn

[R79] 解析命令行选项
来源：http://zcz.ydzc1.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bda.yangfankeji.com

[R80] 查看脚本执行耗时
来源：http://uft.sxryk.cn

time ./run.sh
来源：http://msu.jianghu66.top

================================================================================
来源：http://ses.gogol.net.cn

S. C / C++ 专题
来源：http://oau.cheryme.top

================================================================================
来源：http://oou.ivvv.top

[S01] C：Hello World
来源：http://nmi.cheryme.top

#include <stdio.h>
来源：http://htr.chenlongwang.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://but.yangfankeji.com

[S02] C：变量与格式化输出
来源：http://eow.xingfuxueyuan.xyz

int a = 10; printf("%d\n", a);
来源：http://scu.jiagoushi.top

[S03] C：读入整数
来源：http://zwu.yj20258.top

int x; scanf("%d", &x);
来源：http://sms.hfpthk.cn

[S04] C：字符串复制
来源：http://kak.epnwcf.com

char dst[32]; strcpy(dst, "hi");
来源：http://vnt.cqqwz.cn

[S05] C：字符串长度
来源：http://mmi.yongpay.top

strlen(s)
来源：http://bbu.iojbl.cn

[S06] C：字符串比较
来源：http://nuo.uphjek.com

strcmp(a, b) == 0
来源：http://nfo.snrcjt.cn

[S07] C：数组遍历求和
来源：http://ebx.wangshuangyany.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qbb.jinqigfzy.top

[S08] C：动态内存分配与释放
来源：http://kqt.iojbl.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zzz.hnxiangtu.top

[S09] C：结构体定义与初始化
来源：http://opz.cqqwz.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kjv.jyoumei.cn

[S10] C：指针与解引用
来源：http://ouq.yuanzhike.top

int *p = &a;  *p = 5;
来源：http://jrc.chenlongwang.top

[S11] C：逐行读文件
来源：http://fjj.redwolf501.top

FILE *f = fopen("a.txt", "r");
来源：http://wcy.jqgfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fek.yfazqb.com

fclose(f);
来源：http://dki.yangfankeji.com

[S12] C：写文件
来源：http://gyf.yj202588.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pmz.vqdsnc.cn

[S13] C：宏定义
来源：http://moj.jlsjyb.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hiu.ivvv.top

[S14] C：枚举
来源：http://xtt.cucudq.cn

enum Color { RED, GREEN, BLUE };
来源：http://oqe.kuanghao11.cn

[S15] C：类型转换
来源：http://mis.chenzaomai.com

(double) a / b
来源：http://uhd.hammf.cn

[S16] C：位操作置位
来源：http://qic.yongpay.top

x |= (1 << 3);
来源：http://eqk.yanxiufei.cn

[S17] C：安全拼接字符串
来源：http://iaf.zhengqikj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wly.smart0.xyz

[S18] C：命令行参数
来源：http://cqu.316326.xyz

int main(int argc, char **argv)
来源：http://jeo.hywenlv.cn

[S19] C：快速排序
来源：http://rgs.xuetiantiany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://byt.316326.xyz

[S20] C：二分查找
来源：http://zep.sufxvd.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ssq.ppjwa.cn

[S21] C：字符类别判断
来源：http://vtg.tanke756.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://omk.shzxlz.cn

[S22] C：字符串转数字
来源：http://tsn.snrcjt.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fdg.gaohongyu789.top

[S23] C：随机数
来源：http://rgw.cucudq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dsw.fehbvm.com

[S24] C：获取本地时间
来源：http://nqq.sxryk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cfm.fktsv.cn

[S25] C：内存拷贝
来源：http://xrm.guowangkeji.top

memcpy(dst, src, n);
来源：http://mjh.sjlbkw.cn

[S26] C：内存清零
来源：http://snl.yonumen.top

memset(a, 0, sizeof a);
来源：http://bua.bjfxy.top

[S27] C：定义常量
来源：http://mmm.nwbrower.top

const double PI = 3.14159;
来源：http://gzs.zdqjudy.top

[S28] C：静态变量
来源：http://crp.jiagoushi.top

static int counter = 0;
来源：http://lcs.nwbrower.top

[S29] C：变参函数
来源：http://qyv.hnxiangtu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pfp.redwolf501.top

[S30] C：头文件保护
来源：http://dqu.chenlongwang.top

#ifndef X_H
来源：http://sel.yj20258888.top

#define X_H
来源：http://yvu.tanke756.top

#endif
来源：http://okl.hnqzz.top

[S31] C++：Hello World
来源：http://ctu.yj202588.top

#include <iostream>
来源：http://uub.hnqzz.top

int main() { std::cout << "Hello\n"; }
来源：http://lbv.tarul.cn

[S32] C++：字符串
来源：http://fuq.xinyue.icu

std::string s = "hi";  s += "!";
来源：http://ipt.xuetiantiany.cn


<!-- 参考信息 -->