代发 wailian999

[Q61] 移动平均
来源：http://pve.zhixingplan.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dix.gotoacloud.top

[Q62] 分组占比
来源：http://omm.jiagoushi.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xql.tian-w.cn

[Q63] 开启事务
来源：http://tnu.gogol.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rfu.fengsongda.top

[Q64] 提交事务
来源：http://agq.chenlongwang.top

COMMIT;
来源：http://xjp.sweek.top

[Q65] 回滚事务
来源：http://qpj.zdbjq.cn

ROLLBACK;
来源：http://kgm.ybcxt.top

[Q66] 行锁查询
来源：http://fxj.jiagoushi.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ylr.fengsongda.top

[Q67] 设置隔离级别
来源：http://azq.sjlbkw.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wmf.jiagoushi.top

[Q68] 保存点
来源：http://crl.svipenyu.cn

SAVEPOINT sp1;
来源：http://bnv.haohaochexian.top

ROLLBACK TO sp1;
来源：http://tav.xuetiantiany.cn

[Q69] 查看执行计划
来源：http://cno.nanxuanxn.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fgy.xuetiantiany.cn

[Q70] 更新统计信息
来源：http://ehr.epnwcf.com

ANALYZE TABLE users;
来源：http://nhb.zhixingplan.top

[Q71] 查看建表语句
来源：http://jlm.cheryme.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zxv.shanyushiyangtech.top

[Q72] 查看索引
来源：http://hcu.vqdsnc.cn

SHOW INDEX FROM users;
来源：http://ntf.mhx1999.top

[Q73] 查看表状态
来源：http://gsj.yj20258888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://guu.shuidangran.top

[Q74] 强制使用索引
来源：http://pzb.52xcode.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zhm.jinyuanbaomall.cn

[Q75] 日期格式化
来源：http://phw.fktsv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cmg.ehwqpu.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dix.xingfuxueyuan.xyz

[Q76] 按天统计
来源：http://try.0kj1m.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yvr.9152youxi.cn

[Q77] 时间加减
来源：http://ijw.ywan-chungtsiang.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sav.sxryk.cn

[Q78] 当前时间
来源：http://mvw.yj20258888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://keu.dashuyun.cn

[Q79] 字符串拼接
来源：http://rff.hywenlv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dso.jqgufenzy.top

[Q80] 字符串截取
来源：http://fcr.jinqigufen.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://phi.svipenyu.cn

[Q81] 字符串替换
来源：http://nss.jlsjyb.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xro.pycfn.com

[Q82] 字符长度与字节长度
来源：http://tcp.aibaodan.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://enh.hongshengwenyu.top

[Q83] 大小写转换
来源：http://mkj.wangshuangyany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mms.wangdashe.top

[Q84] 去除首尾空格
来源：http://ecp.yuxming.cn

SELECT TRIM(name) FROM users;
来源：http://xgx.sysykeji.top

[Q85] 数值取整
来源：http://ymx.guowangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://laz.xuanzx.com

[Q86] 读取 JSON 字段
来源：http://lhg.jinqigufen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vky.tarul.cn

[Q87] JSON 字段做条件
来源：http://xvu.gaohongyu789.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qzx.sjlbkw.cn

[Q88] 行转列（条件聚合）
来源：http://wur.wangdashe.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ptl.bjfxy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wxy.chenjidiqi.icu

[Q89] 判断表是否存在
来源：http://fyp.fanxiaobao.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ogh.tarul.cn

[Q90] 生成序号列
来源：http://pwg.cashguo.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xkd.epnwcf.com

================================================================================
来源：http://ird.jiagoushi.top

R. Bash 专题
来源：http://atv.cashguo.top

================================================================================
来源：http://xgt.ppjwa.cn

[R01] shebang 与严格模式
来源：http://get.hcnkem.com

#!/usr/bin/env bash
来源：http://nqi.tarul.cn

set -euo pipefail
来源：http://fpc.wangshuangyany.cn

[R02] 变量赋值与使用
来源：http://mdh.nwbrower.top

name="Tom"; echo "$name"
来源：http://xuq.jlsjyb.cn

[R03] 只读变量
来源：http://cpj.wangshuangyany.cn

readonly PI=3.14
来源：http://uej.feifeiyinyue.top

[R04] 位置参数
来源：http://pnp.xuanzx.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ozj.daxiang520.top

[R05] 参数默认值
来源：http://tot.jlsjyb.cn

name="${1:-default}"
来源：http://jhs.gotoacloud.top

[R06] 判断命令是否存在
来源：http://xug.zhijiandao.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xdh.dashuyun.cn

[R07] if 判断文件
来源：http://gfz.hysaishi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ijh.jinqigufen.top

[R08] 数值比较
来源：http://nsg.ivvv.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tmc.shanyushiyangkeji.top

[R09] 字符串比较
来源：http://blj.ybcxt.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://juy.52xcode.cn

[R10] 正则匹配
来源：http://cqu.nanxuanxn.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pxv.cdnleiting.top

[R11] case 多分支
来源：http://via.hnqzz.top

case "$1" in
来源：http://bpi.yvedp.cn

start) echo "启动" ;;
来源：http://yey.ydjk.org.cn

stop)  echo "停止" ;;
来源：http://wcs.svipenyu.cn

*)     echo "未知命令" ;;
来源：http://iup.bjfxy.top

esac
来源：http://rsv.cqqwz.cn

[R12] for 遍历文件
来源：http://hlj.zhongyouzk.top

for f in *.txt; do echo "$f"; done
来源：http://nga.yuxming.cn

[R13] for 计数循环
来源：http://gdj.yangfankeji.com

for i in {1..10}; do echo "$i"; done
来源：http://jeq.hammf.cn

[R14] C 风格 for
来源：http://uxz.yj202588.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iaa.cqqwz.cn

[R15] while 逐行读文件
来源：http://jkh.zhiwuduotai.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hzm.epnwcf.com

[R16] until 等待条件
来源：http://aql.meibo888.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ajc.shuidangran.top

[R17] 数组定义与取值
来源：http://hsb.sufxvd.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bms.tarul.cn

[R18] 遍历数组
来源：http://skm.pycfn.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://khc.redwolf501.top

[R19] 数组长度
来源：http://agj.chenjidiqi.icu

echo "${#arr[@]}"
来源：http://tnp.cashguo.top

[R20] 关联数组（字典）
来源：http://mkm.cucudq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nwq.chenzaomai.com

[R21] 字符串长度
来源：http://max.yj20258.top

echo "${#s}"
来源：http://ofk.hesvh.cn

[R22] 截取子串
来源：http://dwf.fehbvm.com

echo "${s:0:5}"
来源：http://syq.yuxming.cn

[R23] 字符串替换
来源：http://dwy.hywenlv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nax.yongpay.top

[R24] 大小写转换
来源：http://zoy.jlsjyb.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lrb.bbcook.cn

[R25] 去后缀 / 去前缀
来源：http://khn.hesvh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zej.zhengqikj.top

[R26] 命令替换
来源：http://ehx.tarul.cn

now=$(date +%F); echo "$now"
来源：http://sqw.cashguo.top

[R27] 算术展开
来源：http://squ.fktsv.cn

echo $((1 + 2 * 3))
来源：http://dqm.xuetiantiany.cn

[R28] 浮点运算
来源：http://orn.xuetiantiany.cn

echo "scale=2; 10/3" | bc
来源：http://lpz.havefunace.top

[R29] 定义函数
来源：http://cew.zdbjq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lwe.yangfankeji.com

[R30] 函数返回状态码
来源：http://cem.gogol.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://luf.tarul.cn

[R31] 局部变量
来源：http://vhf.shuidangran.top

f() { local x=1; echo "$x"; }
来源：http://sgy.iojbl.cn

[R32] 参数个数校验
来源：http://mcd.jinyuanbaomall.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://thi.yangfankeji.com

[R33] 捕获错误并提示行号
来源：http://fpx.birdmap.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tee.fanxiaobao.xyz

[R34] 退出时清理
来源：http://iww.316326.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://vla.iojbl.cn

[R35] 后台执行并等待
来源：http://rkg.yfazqb.com

sleep 5 & pid=$!; wait "$pid"
来源：http://cim.ehwqpu.com

[R36] 并发执行多个任务
来源：http://eds.cheryme.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vko.feifeiyinyue.top

[R37] 把输出赋给变量
来源：http://quj.tian-w.cn

files=$(ls -1)
来源：http://swv.mhx1999.top

[R38] 管道串联
来源：http://zob.vqdsnc.cn

cat a.txt | grep -i error | wc -l
来源：http://zsb.hnxiangtu.top

[R39] 重定向标准输出与错误
来源：http://kgx.nanxinkj.top

cmd > out.log 2>&1
来源：http://yoe.tianlin.xyz

[R40] 追加写日志
来源：http://zzi.jinqigufen.top

echo "log" >> out.log
来源：http://xbh.quarkkingdee.top

[R41] 丢弃输出
来源：http://gno.0kj1m.cn

cmd >/dev/null 2>&1
来源：http://hnt.ivvv.top

[R42] 输入重定向
来源：http://oqh.jyoumei.cn

wc -l < a.txt
来源：http://vja.vehdjk.com

[R43] 按名字查找文件
来源：http://xui.gzhubu.top

find . -name "*.log" -type f
来源：http://nub.sysykeji.top

[R44] 按修改时间查找
来源：http://uum.shzxlz.cn

find . -mtime -7 -type f
来源：http://qgq.cdnleiting.top

[R45] 批量删除
来源：http://pxj.feifeiyinyue.top

find . -name "*.tmp" -delete
来源：http://nvr.fanxiaobao.xyz

[R46] 递归替换文件内容
来源：http://azl.vehdjk.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ebd.zhijiandao.cn

[R47] sed 单行替换
来源：http://xms.fengsongda.top

sed -i 's/foo/bar/g' a.txt
来源：http://ius.fehbvm.com

[R48] awk 取指定列
来源：http://maw.jinqigfzy.top

awk '{print $1, $3}' a.txt
来源：http://zrz.andypj.xyz

[R49] awk 带条件
来源：http://gcg.shanyushiyangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bum.xuetiantiany.cn

[R50] awk 求和
来源：http://wna.epnwcf.com

awk '{s += $2} END {print s}' a.txt
来源：http://atj.bbcook.cn

[R51] 排序去重取前几
来源：http://wre.yvedp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://trz.xuanzx.com

[R52] 统计行数
来源：http://kak.ydjk.org.cn

wc -l a.txt
来源：http://uyu.316326.xyz

[R53] 查看文件头与实时尾
来源：http://wqn.gzhubu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://obc.iojbl.cn

[R54] 比较两个文件
来源：http://gdd.hnxiangtu.top

diff a.txt b.txt
来源：http://bgh.yj202588.top

[R55] 压缩与解压
来源：http://fmp.bbcook.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://evo.ivvv.top

[R56] 远程拷贝
来源：http://mfv.fengsongda.top

scp file user@host:/path/
来源：http://lua.zdbjq.cn

[R57] 远程执行命令
来源：http://rwg.c1oappe.top

ssh user@host 'uptime'
来源：http://ofm.mhx1999.top

[R58] 下载文件
来源：http://jun.yueranfly.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xhc.cheryme.top

[R59] 发 POST JSON
来源：http://ztw.nanxinkj.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://trw.ehwqpu.com

[R60] 只看 HTTP 状态码
来源：http://mlt.yfazqb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iin.yuxming.cn

[R61] 磁盘占用
来源：http://mxs.redwolf501.top

df -h;  du -sh *
来源：http://cji.hcnkem.com

[R62] 找最占空间的文件
来源：http://rqi.vehdjk.com

du -ah . | sort -rh | head -10
来源：http://fzz.yfazqb.com

[R63] 内存与进程
来源：http://gcw.yj20258888.top

free -h;  ps aux | grep nginx
来源：http://kvt.daria6918.cn

[R64] 结束进程
来源：http://plq.nwbrower.top

kill -9 $(pgrep -f app.py)
来源：http://rsf.hywenlv.cn

[R65] 查看端口占用
来源：http://gbq.jyoumei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yws.yuanzhike.top

[R66] 定时任务
来源：http://mkq.hnqzz.top

crontab -e;  crontab -l
来源：http://xfz.tianlin.xyz

[R67] 生成随机十六进制串
来源：http://feg.ivvv.top

openssl rand -hex 16
来源：http://jst.cashguo.top

[R68] 计算文件校验值
来源：http://ehc.xylfe.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yaj.chenlongwang.top

[R69] 生成随机密码
来源：http://cmu.birdmap.top

head -c 16 /dev/urandom | base64
来源：http://rba.yvedp.cn

[R70] 时间戳与互转
来源：http://esy.xziqi.cn

date +%s;  date -d @1700000000
来源：http://xdu.zhongyouzk.top

[R71] 日期格式化
来源：http://sli.wangshuangyany.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jmm.ppjwa.cn

[R72] 等待端口就绪
来源：http://lng.xinyue.icu

until nc -z localhost 3306; do sleep 1; done
来源：http://elu.316326.xyz

[R73] 分割大日志
来源：http://jdb.zdbjq.cn

split -l 1000 big.log part_
来源：http://itu.sweek.top

[R74] 批量重命名
来源：http://xbx.316326.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qtf.52xcode.cn

[R75] 导出环境变量
来源：http://bnr.ydzc1.top

export PATH="$HOME/bin:$PATH"
来源：http://lff.yuxming.cn

[R76] 使用临时文件
来源：http://zpc.zhixingplan.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tgc.zycfv.cn

[R77] 读取用户输入
来源：http://fav.zdbjq.cn

read -rp "请输入: " ans
来源：http://xot.sufxvd.cn

[R78] 交互式菜单
来源：http://qqh.ctjpmb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://fth.ctjpmb.com

[R79] 解析命令行选项
来源：http://ryd.zhaomingkeji.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://coi.yj20258888.top

[R80] 查看脚本执行耗时
来源：http://lyl.haohaochexian.top

time ./run.sh
来源：http://ydc.snrcjt.cn

================================================================================
来源：http://gur.mhx1999.top

S. C / C++ 专题
来源：http://xvy.jinghuilouyu.cn

================================================================================
来源：http://hsp.hongshengwenyu.top

[S01] C：Hello World
来源：http://iou.mhx1999.top

#include <stdio.h>
来源：http://cdi.nanxuanxn.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xxg.tanke756.top

[S02] C：变量与格式化输出
来源：http://cso.pycfn.com

int a = 10; printf("%d\n", a);
来源：http://zrm.smart0.xyz

[S03] C：读入整数
来源：http://bke.cashguo.top

int x; scanf("%d", &x);
来源：http://hhk.hysaishi.cn

[S04] C：字符串复制
来源：http://jlf.ybcxt.top

char dst[32]; strcpy(dst, "hi");
来源：http://hxl.shanyushiyangtech.top

[S05] C：字符串长度
来源：http://kgt.0kj1m.cn

strlen(s)
来源：http://iwu.tarul.cn

[S06] C：字符串比较
来源：http://itx.xuetiantiany.cn

strcmp(a, b) == 0
来源：http://mce.birdmap.top

[S07] C：数组遍历求和
来源：http://ips.uphjek.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dlk.hnxiangtu.top

[S08] C：动态内存分配与释放
来源：http://bji.jinghuilouyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jza.xziqi.cn

[S09] C：结构体定义与初始化
来源：http://ymd.zdqjudy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kjy.guannengcc.top

[S10] C：指针与解引用
来源：http://dmf.xinyue.icu

int *p = &a;  *p = 5;
来源：http://buw.redwolf501.top

[S11] C：逐行读文件
来源：http://bzb.zdbjq.cn

FILE *f = fopen("a.txt", "r");
来源：http://ujz.dashuyun.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://unl.gzhubu.top

fclose(f);
来源：http://jgq.kuanghao11.cn

[S12] C：写文件
来源：http://mli.xingfuxueyuan.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kcr.havefunace.top

[S13] C：宏定义
来源：http://evy.jyoumei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jad.cdnleiting.top

[S14] C：枚举
来源：http://qmn.uphjek.com

enum Color { RED, GREEN, BLUE };
来源：http://mop.hcnkem.com

[S15] C：类型转换
来源：http://asf.tianlin.xyz

(double) a / b
来源：http://cvk.yj202588.top

[S16] C：位操作置位
来源：http://tih.guannengcc.top

x |= (1 << 3);
来源：http://bkv.pengpengdd.cyou

[S17] C：安全拼接字符串
来源：http://qtf.snrcjt.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fma.xingfuxueyuan.xyz

[S18] C：命令行参数
来源：http://xik.yj202588.top

int main(int argc, char **argv)
来源：http://obf.pycfn.com

[S19] C：快速排序
来源：http://kaq.gotoacloud.top

qsort(a, n, sizeof(int), cmp);
来源：http://icz.jyoumei.cn

[S20] C：二分查找
来源：http://plt.yj20258.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gqo.meibo888.top

[S21] C：字符类别判断
来源：http://cod.hnqzz.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jui.jlsjyb.cn

[S22] C：字符串转数字
来源：http://skf.ppjwa.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bcu.cdnleiting.top

[S23] C：随机数
来源：http://dbv.jinghuilouyu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rwz.yj20258888.top

[S24] C：获取本地时间
来源：http://pmy.pycfn.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xqc.zhiwuduotai.top

[S25] C：内存拷贝
来源：http://yhx.sweek.top

memcpy(dst, src, n);
来源：http://cpy.ctjpmb.com

[S26] C：内存清零
来源：http://lly.nwbrower.top

memset(a, 0, sizeof a);
来源：http://iqg.shanyushiyangkeji.top

[S27] C：定义常量
来源：http://efg.yvedp.cn

const double PI = 3.14159;
来源：http://twz.meibo888.top

[S28] C：静态变量
来源：http://tjd.zhijiandao.cn

static int counter = 0;
来源：http://qgw.zhixingplan.top

[S29] C：变参函数
来源：http://bgd.gaohongyu789.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fkl.birdmap.top

[S30] C：头文件保护
来源：http://rys.zhiwuduotai.top

#ifndef X_H
来源：http://qba.sweek.top

#define X_H
来源：http://bav.zhoulong.xyz

#endif
来源：http://owr.jinqigufen.top

[S31] C++：Hello World
来源：http://jan.xuanzx.com


<!-- 参考信息 -->