代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nms.fanxiaobao.xyz

[Q60] 取上一行 / 下一行
来源：http://fue.yongpay.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://epb.jinghuilouyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pnv.dashuyun.cn

[Q61] 移动平均
来源：http://pgy.guannengcc.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cre.yuxming.cn

[Q62] 分组占比
来源：http://cvd.sysykeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wla.guowangkeji.top

[Q63] 开启事务
来源：http://kpm.sxryk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wmu.52xcode.cn

[Q64] 提交事务
来源：http://epv.9152youxi.cn

COMMIT;
来源：http://dmd.guowangkeji.top

[Q65] 回滚事务
来源：http://dka.aibaodan.cn

ROLLBACK;
来源：http://sfq.yj20258.top

[Q66] 行锁查询
来源：http://hhk.cheryme.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ias.316326.xyz

[Q67] 设置隔离级别
来源：http://mui.xinyue.icu

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://srh.0kj1m.cn

[Q68] 保存点
来源：http://pwf.uphjek.com

SAVEPOINT sp1;
来源：http://dso.hnxiangtu.top

ROLLBACK TO sp1;
来源：http://zco.ydjk.org.cn

[Q69] 查看执行计划
来源：http://vhs.hammf.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ygm.zhongyouzk.top

[Q70] 更新统计信息
来源：http://dxi.yfazqb.com

ANALYZE TABLE users;
来源：http://zox.shuidangran.top

[Q71] 查看建表语句
来源：http://mis.ctjpmb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dye.uphjek.com

[Q72] 查看索引
来源：http://qfh.yj202588.top

SHOW INDEX FROM users;
来源：http://dho.zhijiandao.cn

[Q73] 查看表状态
来源：http://ona.yj202588.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zhp.zhoulong.xyz

[Q74] 强制使用索引
来源：http://ggv.c1oappe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://unl.guowangkeji.top

[Q75] 日期格式化
来源：http://iru.ehwqpu.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://inn.hnqzz.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gov.gogol.net.cn

[Q76] 按天统计
来源：http://qso.xingfuxueyuan.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xze.aizwys.cn

[Q77] 时间加减
来源：http://djo.quarkkingdee.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tir.guowangkeji.top

[Q78] 当前时间
来源：http://nox.yuxming.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bdm.andypj.xyz

[Q79] 字符串拼接
来源：http://jyv.fktsv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://icp.c1oappe.top

[Q80] 字符串截取
来源：http://boa.316326.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eld.fengsongda.top

[Q81] 字符串替换
来源：http://mer.quarkkingdee.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dwa.uphjek.com

[Q82] 字符长度与字节长度
来源：http://qsc.dianchejie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fif.yueranfly.top

[Q83] 大小写转换
来源：http://qaz.yuxming.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jez.bbcook.cn

[Q84] 去除首尾空格
来源：http://xiv.cheryme.top

SELECT TRIM(name) FROM users;
来源：http://tel.sufxvd.cn

[Q85] 数值取整
来源：http://kcl.52xcode.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kak.shangyingyoupin.top

[Q86] 读取 JSON 字段
来源：http://xyb.gotoacloud.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xai.hongshengwenyu.top

[Q87] JSON 字段做条件
来源：http://lum.9152youxi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uxb.jqgfzy.top

[Q88] 行转列（条件聚合）
来源：http://cja.fanxiaobao.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kxd.0kj1m.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://htn.xziqi.cn

[Q89] 判断表是否存在
来源：http://mpd.guowangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qxr.zdqjudy.top

[Q90] 生成序号列
来源：http://hyp.epnwcf.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rwi.jiagoushi.top

================================================================================
来源：http://quv.dianchejie.cn

R. Bash 专题
来源：http://zng.zhiwuduotai.top

================================================================================
来源：http://dkq.c1oappe.top

[R01] shebang 与严格模式
来源：http://eyp.snrcjt.cn

#!/usr/bin/env bash
来源：http://pni.daxiang520.top

set -euo pipefail
来源：http://fof.xuanzx.com

[R02] 变量赋值与使用
来源：http://kef.jqgfzy.top

name="Tom"; echo "$name"
来源：http://slt.aizwys.cn

[R03] 只读变量
来源：http://ekc.316326.xyz

readonly PI=3.14
来源：http://xrx.shangyingyoupin.top

[R04] 位置参数
来源：http://sfi.sxryk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://srf.yangfankeji.com

[R05] 参数默认值
来源：http://ube.hfpthk.cn

name="${1:-default}"
来源：http://drk.yvedp.cn

[R06] 判断命令是否存在
来源：http://pyy.hfpthk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hwu.bjfxy.top

[R07] if 判断文件
来源：http://wpj.birdmap.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jzg.zhengqikj.top

[R08] 数值比较
来源：http://jym.shanyushiyangkeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ncx.sjlbkw.cn

[R09] 字符串比较
来源：http://fmd.jinqigfzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ame.gotoacloud.top

[R10] 正则匹配
来源：http://abq.jlsjyb.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://stu.fehbvm.com

[R11] case 多分支
来源：http://rso.xuanzx.com

case "$1" in
来源：http://mvk.dashuyun.cn

start) echo "启动" ;;
来源：http://inm.yangfankeji.com

stop)  echo "停止" ;;
来源：http://acv.vqdsnc.cn

*)     echo "未知命令" ;;
来源：http://xxw.yvedp.cn

esac
来源：http://xam.zhoulong.xyz

[R12] for 遍历文件
来源：http://ppj.zhoulong.xyz

for f in *.txt; do echo "$f"; done
来源：http://hns.snrcjt.cn

[R13] for 计数循环
来源：http://mzs.tianlin.xyz

for i in {1..10}; do echo "$i"; done
来源：http://zkr.cqqwz.cn

[R14] C 风格 for
来源：http://boc.hnqzz.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xov.chenzaomai.com

[R15] while 逐行读文件
来源：http://fiq.hcnkem.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xvm.ivvv.top

[R16] until 等待条件
来源：http://cow.yangfankeji.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qfr.wangshuangyany.cn

[R17] 数组定义与取值
来源：http://yql.havefunace.top

arr=(a b c); echo "${arr[0]}"
来源：http://auk.yueranfly.top

[R18] 遍历数组
来源：http://bov.jinyuanbaomall.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://icv.chenzaomai.com

[R19] 数组长度
来源：http://ahl.yvedp.cn

echo "${#arr[@]}"
来源：http://hkt.hcnkem.com

[R20] 关联数组（字典）
来源：http://tfb.mhx1999.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vmi.yfazqb.com

[R21] 字符串长度
来源：http://icc.ehwqpu.com

echo "${#s}"
来源：http://wdk.kuanghao11.cn

[R22] 截取子串
来源：http://faa.tarul.cn

echo "${s:0:5}"
来源：http://awv.yj20258.top

[R23] 字符串替换
来源：http://tpp.yj20258888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dyh.cdnleiting.top

[R24] 大小写转换
来源：http://own.cucudq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xfg.xuetiantiany.cn

[R25] 去后缀 / 去前缀
来源：http://jdx.yj20258.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mky.zhixingplan.top

[R26] 命令替换
来源：http://fbj.ywan-chungtsiang.top

now=$(date +%F); echo "$now"
来源：http://bbw.zhengqikj.top

[R27] 算术展开
来源：http://cpu.hywenlv.cn

echo $((1 + 2 * 3))
来源：http://tkl.svipenyu.cn

[R28] 浮点运算
来源：http://jqw.fehbvm.com

echo "scale=2; 10/3" | bc
来源：http://vme.aibaodan.cn

[R29] 定义函数
来源：http://rrk.xziqi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bgs.shzxlz.cn

[R30] 函数返回状态码
来源：http://eav.guowangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://mtr.xziqi.cn

[R31] 局部变量
来源：http://iit.snrcjt.cn

f() { local x=1; echo "$x"; }
来源：http://dzm.hcnkem.com

[R32] 参数个数校验
来源：http://mot.hnqzz.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cul.52xcode.cn

[R33] 捕获错误并提示行号
来源：http://suz.iojbl.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://llw.gotoacloud.top

[R34] 退出时清理
来源：http://bts.zdbjq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lec.hongshengwenyu.top

[R35] 后台执行并等待
来源：http://iyl.zhijiandao.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://txr.gzhubu.top

[R36] 并发执行多个任务
来源：http://tvs.yj20258888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wtr.tarul.cn

[R37] 把输出赋给变量
来源：http://ccy.gotoacloud.top

files=$(ls -1)
来源：http://vna.chenzaomai.com

[R38] 管道串联
来源：http://lib.nwbrower.top

cat a.txt | grep -i error | wc -l
来源：http://icm.svipenyu.cn

[R39] 重定向标准输出与错误
来源：http://qev.dashuyun.cn

cmd > out.log 2>&1
来源：http://zlc.zhongyouzk.top

[R40] 追加写日志
来源：http://uim.daria6918.cn

echo "log" >> out.log
来源：http://gfa.tian-w.cn

[R41] 丢弃输出
来源：http://vuj.cdnleiting.top

cmd >/dev/null 2>&1
来源：http://lts.cdnleiting.top

[R42] 输入重定向
来源：http://cex.chenjidiqi.icu

wc -l < a.txt
来源：http://jkp.jinqigfzy.top

[R43] 按名字查找文件
来源：http://xke.bbcook.cn

find . -name "*.log" -type f
来源：http://wfv.tanke756.top

[R44] 按修改时间查找
来源：http://uew.jianghu66.top

find . -mtime -7 -type f
来源：http://zhp.hammf.cn

[R45] 批量删除
来源：http://ddr.ppjwa.cn

find . -name "*.tmp" -delete
来源：http://idg.feifeiyinyue.top

[R46] 递归替换文件内容
来源：http://szp.zdqjudy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hah.tanke756.top

[R47] sed 单行替换
来源：http://uvl.gaohongyu789.top

sed -i 's/foo/bar/g' a.txt
来源：http://hsz.xziqi.cn

[R48] awk 取指定列
来源：http://idj.jinqigfzy.top

awk '{print $1, $3}' a.txt
来源：http://zat.sxryk.cn

[R49] awk 带条件
来源：http://cgr.zhijiandao.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://otj.gzhubu.top

[R50] awk 求和
来源：http://nqg.yonumen.top

awk '{s += $2} END {print s}' a.txt
来源：http://rgp.ydzc1.top

[R51] 排序去重取前几
来源：http://cnb.chenlongwang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://irm.jqgufenzy.top

[R52] 统计行数
来源：http://lyh.aibaodan.cn

wc -l a.txt
来源：http://osw.gzhubu.top

[R53] 查看文件头与实时尾
来源：http://gox.ppjwa.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://psp.yj20258888.top

[R54] 比较两个文件
来源：http://awz.andypj.xyz

diff a.txt b.txt
来源：http://els.xinyue.icu

[R55] 压缩与解压
来源：http://adl.tianlin.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uzi.daxiang520.top

[R56] 远程拷贝
来源：http://yeq.jqgfzy.top

scp file user@host:/path/
来源：http://dly.xziqi.cn

[R57] 远程执行命令
来源：http://fvd.xylfe.cn

ssh user@host 'uptime'
来源：http://ccw.zhijiandao.cn

[R58] 下载文件
来源：http://irn.gogol.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fsk.svipenyu.cn

[R59] 发 POST JSON
来源：http://epm.sysykeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fde.fengsongda.top

[R60] 只看 HTTP 状态码
来源：http://zbg.meibo888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gjt.yfazqb.com

[R61] 磁盘占用
来源：http://kyj.ivvv.top

df -h;  du -sh *
来源：http://rle.nanxinkj.top

[R62] 找最占空间的文件
来源：http://swx.wangshuangyany.cn

du -ah . | sort -rh | head -10
来源：http://ewv.zhoulong.xyz

[R63] 内存与进程
来源：http://xuk.xinyue.icu

free -h;  ps aux | grep nginx
来源：http://iue.gzhubu.top

[R64] 结束进程
来源：http://rvk.havefunace.top

kill -9 $(pgrep -f app.py)
来源：http://bkw.xuetiantiany.cn

[R65] 查看端口占用
来源：http://mhd.yuanzhike.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oqu.nwbrower.top

[R66] 定时任务
来源：http://zgw.hfpthk.cn

crontab -e;  crontab -l
来源：http://cvn.hfpthk.cn

[R67] 生成随机十六进制串
来源：http://iel.guannengcc.top

openssl rand -hex 16
来源：http://aie.hywenlv.cn

[R68] 计算文件校验值
来源：http://zvk.uphjek.com

sha256sum a.txt;  md5sum a.txt
来源：http://ols.aibaodan.cn

[R69] 生成随机密码
来源：http://zea.kuanghao11.cn

head -c 16 /dev/urandom | base64
来源：http://wfb.zdqjudy.top

[R70] 时间戳与互转
来源：http://oul.xuanzx.com

date +%s;  date -d @1700000000
来源：http://puc.cqqwz.cn

[R71] 日期格式化
来源：http://sof.haohaochexian.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lgz.dianchejie.cn

[R72] 等待端口就绪
来源：http://qiw.c1oappe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://myp.zhongyouzk.top

[R73] 分割大日志
来源：http://sis.ywan-chungtsiang.top

split -l 1000 big.log part_
来源：http://hcs.yj20258.top

[R74] 批量重命名
来源：http://lhq.sufxvd.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qaz.dashuyun.cn

[R75] 导出环境变量
来源：http://oqt.xylfe.cn

export PATH="$HOME/bin:$PATH"
来源：http://hbc.chenzaomai.com

[R76] 使用临时文件
来源：http://sst.tanke756.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fsi.pengpengdd.cyou

[R77] 读取用户输入
来源：http://hcl.zhijiandao.cn

read -rp "请输入: " ans
来源：http://tev.zhijiandao.cn

[R78] 交互式菜单
来源：http://vuf.gogol.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kkm.daria6918.cn

[R79] 解析命令行选项
来源：http://djp.zhijiandao.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vhi.hywenlv.cn

[R80] 查看脚本执行耗时
来源：http://vsz.aizwys.cn

time ./run.sh
来源：http://rhg.jyoumei.cn

================================================================================
来源：http://rsx.birdmap.top

S. C / C++ 专题
来源：http://vsn.sysykeji.top

================================================================================
来源：http://iab.chenzaomai.com

[S01] C：Hello World
来源：http://xmm.ivvv.top

#include <stdio.h>
来源：http://ume.zhijiandao.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://acm.chenlongwang.top

[S02] C：变量与格式化输出
来源：http://uqc.yvedp.cn

int a = 10; printf("%d\n", a);
来源：http://vvw.daria6918.cn

[S03] C：读入整数
来源：http://ptc.pengpengdd.cyou

int x; scanf("%d", &x);
来源：http://cin.snrcjt.cn

[S04] C：字符串复制
来源：http://rqt.chenjidiqi.icu

char dst[32]; strcpy(dst, "hi");
来源：http://dfp.chenlongwang.top

[S05] C：字符串长度
来源：http://wrq.epnwcf.com

strlen(s)
来源：http://imo.mhx1999.top

[S06] C：字符串比较
来源：http://lvx.cheryme.top

strcmp(a, b) == 0
来源：http://dxd.ppjwa.cn

[S07] C：数组遍历求和
来源：http://qxw.jinqigufen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dhu.hesvh.cn

[S08] C：动态内存分配与释放
来源：http://sme.gogol.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oxf.ydzc1.top

[S09] C：结构体定义与初始化
来源：http://bpx.jqgfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zjp.zhoulong.xyz

[S10] C：指针与解引用
来源：http://lda.zhongyouzk.top

int *p = &a;  *p = 5;
来源：http://gca.nanxuanxn.top

[S11] C：逐行读文件
来源：http://nlh.guowangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://jdj.yuanzhike.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rpv.yonumen.top

fclose(f);
来源：http://rxl.yfazqb.com

[S12] C：写文件
来源：http://lpq.vehdjk.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gag.fehbvm.com

[S13] C：宏定义
来源：http://lgr.epnwcf.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wwn.c1oappe.top

[S14] C：枚举
来源：http://iww.guowangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://xzv.aibaodan.cn

[S15] C：类型转换
来源：http://uaf.chenjidiqi.icu

(double) a / b
来源：http://ioe.jinqigfzy.top

[S16] C：位操作置位
来源：http://cxu.sjlbkw.cn

x |= (1 << 3);
来源：http://wee.aibaodan.cn

[S17] C：安全拼接字符串
来源：http://goa.wangshuangyany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://irk.hysaishi.cn

[S18] C：命令行参数
来源：http://kiw.zhongyouzk.top

int main(int argc, char **argv)
来源：http://paj.ybcxt.top

[S19] C：快速排序
来源：http://usd.gogol.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ulv.snrcjt.cn

[S20] C：二分查找
来源：http://jsp.52xcode.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zzz.epnwcf.com

[S21] C：字符类别判断
来源：http://avp.bjfxy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wkw.ctjpmb.com

[S22] C：字符串转数字
来源：http://kcc.hnqzz.top

atoi("42");  strtod("3.14", NULL);
来源：http://vze.tarul.cn

[S23] C：随机数
来源：http://llc.fehbvm.com

srand(time(NULL));  int r = rand() % 100;
来源：http://iwf.sufxvd.cn

[S24] C：获取本地时间
来源：http://juf.yuanzhike.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zhb.hongshengwenyu.top

[S25] C：内存拷贝
来源：http://dzg.sufxvd.cn

memcpy(dst, src, n);
来源：http://fqz.wangshuangyany.cn

[S26] C：内存清零
来源：http://tcs.shangyingyoupin.top

memset(a, 0, sizeof a);
来源：http://ysn.yj202588.top

[S27] C：定义常量
来源：http://lpc.chenjidiqi.icu

const double PI = 3.14159;
来源：http://jli.zhoulong.xyz

[S28] C：静态变量
来源：http://oln.316326.xyz

static int counter = 0;
来源：http://eqg.hnqzz.top

[S29] C：变参函数
来源：http://xhz.ivvv.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nbq.kuanghao11.cn

[S30] C：头文件保护
来源：http://bke.xuetiantiany.cn


<!-- 参考信息 -->