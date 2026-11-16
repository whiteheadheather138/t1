代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hfe.zhaomingkeji.xyz

[Q54] 清空表
来源：http://pcw.sweek.top

TRUNCATE TABLE logs;
来源：http://rqy.guowangkeji.top

[Q55] 排名（并列占位）
来源：http://jcv.yvedp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nyj.epnwcf.com

[Q56] 密集排名（并列不占位）
来源：http://olo.smart0.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tdx.xingfuxueyuan.xyz

[Q57] 行号
来源：http://vbq.hfpthk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uck.ywan-chungtsiang.top

[Q58] 累计求和
来源：http://zjq.yvedp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aos.jlsjyb.cn

[Q59] 分组内累计
来源：http://cpa.sxryk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jdy.9152youxi.cn

[Q60] 取上一行 / 下一行
来源：http://zjp.sysykeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wjv.52xcode.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ucs.hnqzz.top

[Q61] 移动平均
来源：http://apq.hammf.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xhv.yonumen.top

[Q62] 分组占比
来源：http://fre.yuxming.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oro.iojbl.cn

[Q63] 开启事务
来源：http://slv.316326.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://opj.52xcode.cn

[Q64] 提交事务
来源：http://qcd.yuxming.cn

COMMIT;
来源：http://ejt.gzhubu.top

[Q65] 回滚事务
来源：http://qyz.9152youxi.cn

ROLLBACK;
来源：http://eif.havefunace.top

[Q66] 行锁查询
来源：http://ewu.sysykeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gbk.yj20258888.top

[Q67] 设置隔离级别
来源：http://lon.chenzaomai.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dsq.hammf.cn

[Q68] 保存点
来源：http://jlv.feifeiyinyue.top

SAVEPOINT sp1;
来源：http://fya.snrcjt.cn

ROLLBACK TO sp1;
来源：http://foj.jianghu66.top

[Q69] 查看执行计划
来源：http://lfi.jinqigfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://usc.havefunace.top

[Q70] 更新统计信息
来源：http://xdd.tarul.cn

ANALYZE TABLE users;
来源：http://elj.aibaodan.cn

[Q71] 查看建表语句
来源：http://amx.zycfv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cjt.yvedp.cn

[Q72] 查看索引
来源：http://amz.nanxinkj.top

SHOW INDEX FROM users;
来源：http://hag.pycfn.com

[Q73] 查看表状态
来源：http://rgz.gogol.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://our.kuanghao11.cn

[Q74] 强制使用索引
来源：http://qkb.hnxiangtu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fzo.feifeiyinyue.top

[Q75] 日期格式化
来源：http://soo.ppjwa.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ccs.52xcode.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dcl.uphjek.com

[Q76] 按天统计
来源：http://cgu.zhixingplan.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hwf.tarul.cn

[Q77] 时间加减
来源：http://zzs.nanxinkj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fpf.sxryk.cn

[Q78] 当前时间
来源：http://kax.yj20258888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qbb.kuanghao11.cn

[Q79] 字符串拼接
来源：http://ulr.havefunace.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ucx.jinqigufen.top

[Q80] 字符串截取
来源：http://fdo.jqgfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ztr.bbcook.cn

[Q81] 字符串替换
来源：http://jrc.yuanzhike.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tlw.sweek.top

[Q82] 字符长度与字节长度
来源：http://ogc.tianlin.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ylf.uphjek.com

[Q83] 大小写转换
来源：http://oje.yonumen.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mls.snrcjt.cn

[Q84] 去除首尾空格
来源：http://hkv.shanyushiyangkeji.top

SELECT TRIM(name) FROM users;
来源：http://npm.yj202588.top

[Q85] 数值取整
来源：http://kup.vqdsnc.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zjl.xinyue.icu

[Q86] 读取 JSON 字段
来源：http://sba.epnwcf.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cjh.yj20258888.top

[Q87] JSON 字段做条件
来源：http://ity.ywan-chungtsiang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gly.ppjwa.cn

[Q88] 行转列（条件聚合）
来源：http://pju.jinqigfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gve.hammf.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://idx.andypj.xyz

[Q89] 判断表是否存在
来源：http://isj.fanxiaobao.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ozb.hfpthk.cn

[Q90] 生成序号列
来源：http://rvw.jinqigfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wgb.guannengcc.top

================================================================================
来源：http://hth.chenjidiqi.icu

R. Bash 专题
来源：http://dsu.vehdjk.com

================================================================================
来源：http://vfm.guowangkeji.top

[R01] shebang 与严格模式
来源：http://uwr.0kj1m.cn

#!/usr/bin/env bash
来源：http://ybk.zhiwuduotai.top

set -euo pipefail
来源：http://txh.cdnleiting.top

[R02] 变量赋值与使用
来源：http://elv.hesvh.cn

name="Tom"; echo "$name"
来源：http://emo.sufxvd.cn

[R03] 只读变量
来源：http://vyk.yj20258888.top

readonly PI=3.14
来源：http://amf.hfpthk.cn

[R04] 位置参数
来源：http://aan.iojbl.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ipe.jiagoushi.top

[R05] 参数默认值
来源：http://pyb.chenzaomai.com

name="${1:-default}"
来源：http://gva.dianchejie.cn

[R06] 判断命令是否存在
来源：http://kec.ybcxt.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pvf.jqgufenzy.top

[R07] if 判断文件
来源：http://cxp.wangdashe.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ldi.ywan-chungtsiang.top

[R08] 数值比较
来源：http://gau.dianchejie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vrt.kuanghao11.cn

[R09] 字符串比较
来源：http://ygn.gogol.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zbg.316326.xyz

[R10] 正则匹配
来源：http://nwy.fanxiaobao.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pbb.pengpengdd.cyou

[R11] case 多分支
来源：http://kmc.chenzaomai.com

case "$1" in
来源：http://vib.mhx1999.top

start) echo "启动" ;;
来源：http://oqd.snrcjt.cn

stop)  echo "停止" ;;
来源：http://qdp.0kj1m.cn

*)     echo "未知命令" ;;
来源：http://wli.ybcxt.top

esac
来源：http://fkt.nanxinkj.top

[R12] for 遍历文件
来源：http://ifj.chenlongwang.top

for f in *.txt; do echo "$f"; done
来源：http://cqh.tianlin.xyz

[R13] for 计数循环
来源：http://nzb.haohaochexian.top

for i in {1..10}; do echo "$i"; done
来源：http://psu.smart0.xyz

[R14] C 风格 for
来源：http://crl.jinghuilouyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://clt.aizwys.cn

[R15] while 逐行读文件
来源：http://yuh.zhijiandao.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pti.snrcjt.cn

[R16] until 等待条件
来源：http://zjj.birdmap.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xss.nanxinkj.top

[R17] 数组定义与取值
来源：http://ijg.fktsv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gic.mhx1999.top

[R18] 遍历数组
来源：http://agy.xziqi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mhp.bbcook.cn

[R19] 数组长度
来源：http://hfj.shanyushiyangtech.top

echo "${#arr[@]}"
来源：http://jtm.tian-w.cn

[R20] 关联数组（字典）
来源：http://tiz.pycfn.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xeo.shuidangran.top

[R21] 字符串长度
来源：http://xez.chenlongwang.top

echo "${#s}"
来源：http://duq.ppjwa.cn

[R22] 截取子串
来源：http://vib.ctjpmb.com

echo "${s:0:5}"
来源：http://oxl.jianghu66.top

[R23] 字符串替换
来源：http://ofz.wangdashe.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rbu.ctjpmb.com

[R24] 大小写转换
来源：http://fcj.hammf.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jlj.zhoulong.xyz

[R25] 去后缀 / 去前缀
来源：http://ldu.sxryk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nxy.chenzaomai.com

[R26] 命令替换
来源：http://wdt.hammf.cn

now=$(date +%F); echo "$now"
来源：http://kiw.fktsv.cn

[R27] 算术展开
来源：http://fhx.shanyushiyangkeji.top

echo $((1 + 2 * 3))
来源：http://doa.yj20258.top

[R28] 浮点运算
来源：http://hep.ydjk.org.cn

echo "scale=2; 10/3" | bc
来源：http://zwz.hnxiangtu.top

[R29] 定义函数
来源：http://cgh.yanxiufei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://faf.nanxinkj.top

[R30] 函数返回状态码
来源：http://sjo.hongshengwenyu.top

f() { return 0; }; f || echo "失败了"
来源：http://dim.hnxiangtu.top

[R31] 局部变量
来源：http://unb.hesvh.cn

f() { local x=1; echo "$x"; }
来源：http://rtx.shanyushiyangkeji.top

[R32] 参数个数校验
来源：http://fmp.ctjpmb.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://arw.dianchejie.cn

[R33] 捕获错误并提示行号
来源：http://zwo.chenlongwang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://khf.zhongyouzk.top

[R34] 退出时清理
来源：http://taj.zhijiandao.cn

trap 'rm -f "$tmp"' EXIT
来源：http://abl.hesvh.cn

[R35] 后台执行并等待
来源：http://mdx.hnxiangtu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://doy.ydjk.org.cn

[R36] 并发执行多个任务
来源：http://lfd.yanxiufei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kio.redwolf501.top

[R37] 把输出赋给变量
来源：http://alc.jyoumei.cn

files=$(ls -1)
来源：http://jer.feifeiyinyue.top

[R38] 管道串联
来源：http://dsj.redwolf501.top

cat a.txt | grep -i error | wc -l
来源：http://rqb.zhongyouzk.top

[R39] 重定向标准输出与错误
来源：http://kxb.zhaomingkeji.xyz

cmd > out.log 2>&1
来源：http://lnk.wangdashe.top

[R40] 追加写日志
来源：http://skq.mhx1999.top

echo "log" >> out.log
来源：http://ftn.0kj1m.cn

[R41] 丢弃输出
来源：http://yst.ywan-chungtsiang.top

cmd >/dev/null 2>&1
来源：http://vqj.zhengqikj.top

[R42] 输入重定向
来源：http://taw.yfazqb.com

wc -l < a.txt
来源：http://rll.zhoulong.xyz

[R43] 按名字查找文件
来源：http://luv.yvedp.cn

find . -name "*.log" -type f
来源：http://vrm.zhaomingkeji.xyz

[R44] 按修改时间查找
来源：http://qaf.chenzaomai.com

find . -mtime -7 -type f
来源：http://mwd.zhijiandao.cn

[R45] 批量删除
来源：http://zbm.hfpthk.cn

find . -name "*.tmp" -delete
来源：http://mny.tian-w.cn

[R46] 递归替换文件内容
来源：http://crh.yj202588.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lqe.zhengqikj.top

[R47] sed 单行替换
来源：http://svf.sysykeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://dph.yanxiufei.cn

[R48] awk 取指定列
来源：http://hpq.shuidangran.top

awk '{print $1, $3}' a.txt
来源：http://vhl.zhixingplan.top

[R49] awk 带条件
来源：http://wpv.nwbrower.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hyy.hnxiangtu.top

[R50] awk 求和
来源：http://dnj.hnxiangtu.top

awk '{s += $2} END {print s}' a.txt
来源：http://wvk.tianlin.xyz

[R51] 排序去重取前几
来源：http://cch.shuidangran.top

sort a.txt | uniq -c | sort -rn | head
来源：http://eib.yueranfly.top

[R52] 统计行数
来源：http://wxw.chenjidiqi.icu

wc -l a.txt
来源：http://suz.sxryk.cn

[R53] 查看文件头与实时尾
来源：http://kno.ctjpmb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://txy.shangyingyoupin.top

[R54] 比较两个文件
来源：http://hqx.smart0.xyz

diff a.txt b.txt
来源：http://eez.zhengqikj.top

[R55] 压缩与解压
来源：http://hwb.hysaishi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lvi.pycfn.com

[R56] 远程拷贝
来源：http://pox.vehdjk.com

scp file user@host:/path/
来源：http://tsc.fanxiaobao.xyz

[R57] 远程执行命令
来源：http://dgl.sufxvd.cn

ssh user@host 'uptime'
来源：http://bdd.sjlbkw.cn

[R58] 下载文件
来源：http://bom.vehdjk.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vmc.yfazqb.com

[R59] 发 POST JSON
来源：http://qsi.zhaomingkeji.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gij.wangshuangyany.cn

[R60] 只看 HTTP 状态码
来源：http://xwn.zycfv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://shk.fehbvm.com

[R61] 磁盘占用
来源：http://wbw.aizwys.cn

df -h;  du -sh *
来源：http://znv.shanyushiyangkeji.top

[R62] 找最占空间的文件
来源：http://ybi.cdnleiting.top

du -ah . | sort -rh | head -10
来源：http://mbe.nanxuanxn.top

[R63] 内存与进程
来源：http://ind.tarul.cn

free -h;  ps aux | grep nginx
来源：http://hev.kuanghao11.cn

[R64] 结束进程
来源：http://uqw.hcnkem.com

kill -9 $(pgrep -f app.py)
来源：http://qcb.havefunace.top

[R65] 查看端口占用
来源：http://rpb.iojbl.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://use.sjlbkw.cn

[R66] 定时任务
来源：http://lau.yuxming.cn

crontab -e;  crontab -l
来源：http://fuy.sufxvd.cn

[R67] 生成随机十六进制串
来源：http://aja.tianlin.xyz

openssl rand -hex 16
来源：http://xpi.zhijiandao.cn

[R68] 计算文件校验值
来源：http://clh.cqqwz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mtq.316326.xyz

[R69] 生成随机密码
来源：http://otg.redwolf501.top

head -c 16 /dev/urandom | base64
来源：http://ljw.zhiwuduotai.top

[R70] 时间戳与互转
来源：http://hdp.hfpthk.cn

date +%s;  date -d @1700000000
来源：http://bck.zhijiandao.cn

[R71] 日期格式化
来源：http://sfe.xziqi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pkc.hysaishi.cn

[R72] 等待端口就绪
来源：http://xmv.daria6918.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tkz.iojbl.cn

[R73] 分割大日志
来源：http://acb.daxiang520.top

split -l 1000 big.log part_
来源：http://vky.zhixingplan.top

[R74] 批量重命名
来源：http://auo.tanke756.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vij.yfazqb.com

[R75] 导出环境变量
来源：http://xfo.jqgfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://qkm.daxiang520.top

[R76] 使用临时文件
来源：http://sav.redwolf501.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bhc.zdqjudy.top

[R77] 读取用户输入
来源：http://uqz.svipenyu.cn

read -rp "请输入: " ans
来源：http://mkx.dashuyun.cn

[R78] 交互式菜单
来源：http://zfa.shuidangran.top

select opt in a b c; do echo "$opt"; break; done
来源：http://koa.smart0.xyz

[R79] 解析命令行选项
来源：http://uwl.shangyingyoupin.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bwh.pengpengdd.cyou

[R80] 查看脚本执行耗时
来源：http://onr.hammf.cn

time ./run.sh
来源：http://xlk.shuidangran.top

================================================================================
来源：http://aar.daxiang520.top

S. C / C++ 专题
来源：http://zvi.nanxinkj.top

================================================================================
来源：http://axr.uphjek.com

[S01] C：Hello World
来源：http://flf.yfazqb.com

#include <stdio.h>
来源：http://dse.xingfuxueyuan.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://knd.hammf.cn

[S02] C：变量与格式化输出
来源：http://zky.nanxinkj.top

int a = 10; printf("%d\n", a);
来源：http://tho.yanxiufei.cn

[S03] C：读入整数
来源：http://bne.52xcode.cn

int x; scanf("%d", &x);
来源：http://mrk.jinyuanbaomall.cn

[S04] C：字符串复制
来源：http://pxo.sjlbkw.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vnz.havefunace.top

[S05] C：字符串长度
来源：http://ajt.guannengcc.top

strlen(s)
来源：http://hsx.ydjk.org.cn

[S06] C：字符串比较
来源：http://mrf.shangyingyoupin.top

strcmp(a, b) == 0
来源：http://ukl.316326.xyz

[S07] C：数组遍历求和
来源：http://swj.jinqigfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lxi.xylfe.cn

[S08] C：动态内存分配与释放
来源：http://yyg.shanyushiyangtech.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pcu.jinyuanbaomall.cn

[S09] C：结构体定义与初始化
来源：http://fle.tanke756.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dav.jiagoushi.top

[S10] C：指针与解引用
来源：http://jho.smart0.xyz

int *p = &a;  *p = 5;
来源：http://yqp.fengsongda.top

[S11] C：逐行读文件
来源：http://gfw.fanxiaobao.xyz

FILE *f = fopen("a.txt", "r");
来源：http://zcj.yanxiufei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gld.shanyushiyangkeji.top

fclose(f);
来源：http://crz.tanke756.top

[S12] C：写文件
来源：http://xtl.9152youxi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://svz.hesvh.cn

[S13] C：宏定义
来源：http://yai.hfpthk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dta.redwolf501.top

[S14] C：枚举
来源：http://otb.dashuyun.cn

enum Color { RED, GREEN, BLUE };
来源：http://hjy.cdnleiting.top

[S15] C：类型转换
来源：http://usi.yanxiufei.cn

(double) a / b
来源：http://kia.jinyuanbaomall.cn

[S16] C：位操作置位
来源：http://xqz.9152youxi.cn

x |= (1 << 3);
来源：http://uvs.hnqzz.top

[S17] C：安全拼接字符串
来源：http://cpl.cheryme.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wqe.xinyue.icu

[S18] C：命令行参数
来源：http://cwg.chenlongwang.top

int main(int argc, char **argv)
来源：http://udr.dashuyun.cn

[S19] C：快速排序
来源：http://lay.tanke756.top

qsort(a, n, sizeof(int), cmp);
来源：http://pbb.ywan-chungtsiang.top

[S20] C：二分查找
来源：http://kdk.andypj.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kjf.pycfn.com

[S21] C：字符类别判断
来源：http://zab.jinyuanbaomall.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xzs.cqqwz.cn

[S22] C：字符串转数字
来源：http://uwh.hcnkem.com

atoi("42");  strtod("3.14", NULL);
来源：http://cug.ivvv.top

[S23] C：随机数
来源：http://ntb.sjlbkw.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kty.yj202588.top

[S24] C：获取本地时间
来源：http://csi.haohaochexian.top


<!-- 参考信息 -->